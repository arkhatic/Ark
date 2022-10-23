<template>
  <div ref="parentEl" class="flex justify-center items-center w-full">
    <button 
      class="p-1 rounded-full text-white"
      @click="play">
        <svg 
          v-if="!isPlaying"
          data-testid="play" 
          class="w-5 h-5 hover:transform hover:scale-125" 
          fill="#8f8f8f" 
          stroke="currentColor" 
          viewBox="0 0 24 24" 
          xmlns="http://www.w3.org/2000/svg">

          <path 
            stroke-linecap="round" 
            stroke-linejoin="round" 
            stroke-width="0" 
            d="M5 3l14 9-14 9V3z">
          </path>
        </svg>

        <svg 
          v-else
          data-testid="pause" 
          class="w-5 h-5 hover:transform hover:scale-125" 
          fill="#8f8f8f" 
          stroke="#8f8f8f" 
          viewBox="0 0 24 24" 
          xmlns="http://www.w3.org/2000/svg">

          <path 
            stroke-linecap="round" 
            stroke-linejoin="round" 
            stroke-width="4" 
            d="M6 18L18 6M6 6l12 12">
          </path>
        </svg>
    </button>
    <div 
      ref="listenTo" 
      class="block h-2 w-1/3 rounded bg-white/50 opacity-50 cursor-pointer">

      <div 
        :style="'width:'+progress+'%'" 
        class="z-50 absolute h-2 rounded bg-white opacity-100 hover:transform hover:scale-y-125">
      </div>
    </div>
  </div>  
</template>

<script>
export default {
  name: 'MusicPlayer',
  props: {
    source: String
  },
  data() {
    return { 
      isPlaying: false,
      player: new Audio(),

      progress: 0,
      wrapperWidth: 0
    };
  },
  created() {
    this.player.src = this.source;
  },
  mounted() {
    this.wrapperWidth = this.$refs.listenTo.offsetWidth;
    this.player.addEventListener('timeupdate', this.updateProgress);
    this.$refs.listenTo.addEventListener("click", this.getClickPosition, false)
    this.$refs.listenTo.addEventListener("mousedown", this.detectMouseDown, false)
    this.$refs.listenTo.addEventListener("mouseup", this.detectMouseUp, false)
  },
  methods: {
    play() {
      if (this.isPlaying) {
        this.player.pause();
        this.isPlaying = false;
      } else {
        this.player.play();
        this.isPlaying = true;
      }

      this.player.addEventListener('ended', () => {
        this.isPlaying = false;
      });
    },  
    updateProgress() {
      this.progress = (this.player.currentTime / this.player.duration) * 33.3 * (this.$refs.parentEl.clientWidth / window.innerWidth);
    },
    getClickPosition(e) {
      const clickPosition = e.pageX - this.$refs.listenTo.offsetLeft;
      const newTime = (clickPosition / this.wrapperWidth) * this.player.duration;
      this.player.currentTime = newTime;
    },
    detectMouseDown(e){
      e.preventDefault()
      this.$refs.listenTo.addEventListener("mousemove", this.getClickPosition, false)
    },
    detectMouseUp(e){
      this.$refs.listenTo.removeEventListener("mousemove", this.getClickPosition, false)
    },
  }
};
</script>