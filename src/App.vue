<template>
  <Sidebar />
  <!-- landing page -->
  <div className="absolute snap-proximity snap-y overflow-y-scroll overflow-x-hidden h-screen w-screen">
  <div class="dark:bg-black bg-white h-screen snap-start video-wrapper" id="home">
    <video playsinline autoplay muted loop>
      <source src="@/assets/background-video.mp4" type="video/mp4">
    </video>

    <div class="bg-filter h-screen w-screen">
      <div class="flex flex-col justify-center h-full mx-12 text-center items-center lg:items-start xl:text-left lg:mx-24 header">
        <h1 class="text-7xl md:text-8xl lg:text-9xl  text-teal-600 font-display font-black">
          Arkhatic, 
        </h1>
  
        <h1 class="text-5xl md:text-6xl dark:text-white text-black font-extrabold">
          award-winning <br>
          composer and scorer.
        </h1>
  
        <a href="https://linktree.com/arkhatic" class="mt-4 text-2xl text-teal-700 font-extrabold">@arkhatic</a>
      </div>
    </div>
  </div>

  <div class="bg-yellow-800 h-auto p-24 text-center">
    <h1 class="text-3xl lg:text-4xl text-white font-extrabold">
      <span class="italic">Tip:</span> hover the mouse or touch over the left to reveal the menu.</h1>
  </div> 

  <!-- about page -->
  <div class="bg-neutral-200 h-auto p-12 lg:p-24 w-screen" id="about">
    <div class="flex flex-col text-left">
      <h1 class="text-6xl md:text-7xl text-black font-extrabold font-display">
        I have always been learning alone.
      </h1>
      
      <div class="flex flex-row mt-4">
        <p class="text-2xl text-black font-bold mt-4 max-w-full">
          I am composer with with more than 5 years of experience composing screamingly loud and emotive music for games, films, and other media. I have worked on:
          <br>
          <br>
          <ul class="lg:ml-12 list-disc">
            <li>Draft in the woods;
              <iframe src="https://store.steampowered.com/widget/2327730/" frameborder="0" width="100%" height="190" class="mt-4 lg:w-[600px]"></iframe>
            </li>

            <li>Reaper of Gods;</li>

            <li>Raifuejji.
            </li>
          </ul>

          <br>
          <br>

          I have also worked on a few other projects, but I can't talk about them yet. 😅 <br>
          <br>
          <h2 class="text-4xl text-black font-black mb-2">Apart from composing,</h2>
          <p>
            I am a game developer experienced in Unity, Godot and GameMaker, everything from procedural generation to AI programming, with 3 years of experience; <br>
            I also have experience in web development, having worked with Vue.js, React.js and its variations, and Node.js; <br>

            And a <span class="text-red-500">huge</span> fan of the <span class="text-blue-500">fantasy</span> genre, and I love to read books and play games. <br>


          </p> 

        </p>
      </div>
    </div>  
  </div>  

  <div class="bg-red-900 h-auto p-12 lg:p-24 w-screen" id="award">
    <h1 class="text-5xl lg:text-6xl xl:text-7xl text-white font-black font-display">Also, in 2022, I won the Hacelo Corto award for the best film score!</h1>
    <h2 class="text-2xl text-white font-bold mt-4 max-w-full">Hacelo Corto is a festival of short films hosted in Buenos Aires, Argentina. <br>
    Our film, Sonitus, won the award for the best score and special mention of the Jury, for its creative drama and emotive all-out soundtrack. <br>
    But, it would not be possible without the help of my team 💖 </h2>

    <h1 class="text-3xl text-black font-black text-white my-3">Hear the OST below!</h1>
    <div class="bg-black py-10 flex flex-col justify-center items-center text-center rounded-xl bg-yelllow-600">
      <h1 class="text-white px-12 text-4xl lg:text-4xl font-extrabold z-0">Sonitus</h1>

      <div class="z-40 w-screen mt-2">
        <MusicPlayer source='/src/assets/audio/Sonitus.mp3' />
      </div>
    </div>

  </div>

  <!-- partners page -->
  <div class="bg-black p-12 lg:p-24 flex flex-col" id="partners">
    <div>
      <h1 class="text-5xl lg:text-6xl xl:text-7xl text-green-700 font-black font-display">Now, I have another job as well.</h1>

      <h2 class="text-3xl text-white font-extrabold mt-8 lg:mt-4">
        Being a military together with being a composer is a challenge I did not know how to face. <br>
        Nevertheless, We do press on as much as we can.
      </h2>
    </div>
  </div>

  <!-- divisory -->
  <div class="bg-blue-800 h-auto p-24 text-center">
    <h1 class="text-5xl text-white font-extrabold">Then I present to you, my flagship songs.</h1>
  </div> 

  <div class="bg-black h-screen flex flex-col justify-center items-center text-center snap-start" id="solo">
    <img 
      src="https://w.wallhaven.cc/full/76/wallhaven-7669r9.png" 
      class="w-full h-full object-cover opacity-50 absolute z-10 ">

    <h1 class="text-white px-12 text-6xl lg:text-8xl font-extrabold z-0">Solo of the Sea</h1>

    <div class="z-40 w-screen mt-2">
      <MusicPlayer source="/src/assets/audio/SoloSea.mp3" />
    </div>
  </div>

  <div class="bg-black h-screen flex flex-col justify-center items-center text-center snap-start" id="record">
    <img 
      src="https://i.pinimg.com/originals/b7/68/b3/b768b3f7dbbc202d280e0f95c46dfb64.jpg" 
      class="w-full h-full object-cover opacity-50 absolute z-10 ">

    <h1 class="text-white px-12 text-6xl lg:text-8xl font-extrabold z-0">For the Record</h1>

    <div class="z-40 w-screen mt-2">
      <MusicPlayer source="/src/assets/audio/Record.mp3" />
    </div>
  </div>

  <div class="bg-black h-screen flex flex-col justify-center items-center text-center snap-start" id="angels">
    <img 
      src="https://images4.alphacoders.com/177/thumb-1920-177128.jpg" 
      class="w-full h-full object-cover opacity-50 absolute z-10 ">

    <h1 class="text-white px-12 text-6xl lg:text-8xl font-extrabold z-0">Scarborough Fair</h1>

    <div class="z-40 w-screen mt-2">
      <MusicPlayer source="/src/assets/audio/Jasmine.wav" />
    </div>
  </div>

  <!-- the undead commander -->
  <div class="bg-black h-screen flex flex-col justify-center items-center text-center snap-start" id="undead-commander">
    <img 
      src="https://images.pexels.com/photos/1054218/pexels-photo-1054218.jpeg?cs=srgb&dl=pexels-stywo-1054218.jpg" 
      class="w-full h-full object-cover opacity-50 absolute z-10 ">

    <h1 class="text-white px-12 text-6xl lg:text-8xl font-extrabold z-0">NCS Classic</h1>

    <div class="z-40 w-screen mt-2">
      <MusicPlayer source="/src/assets/audio/Appear.mp3" />
    </div>
  </div>

  <!-- cantus of requiem -->
  <div class="bg-black h-screen flex flex-col justify-center items-center text-center snap-start" id="awoken">
    <img 
      src="https://r4.wallpaperflare.com/wallpaper/432/899/621/fantasy-art-clouds-digital-art-futuristic-wallpaper-8d1bdf2ceb7791f3e2be17e2500dcba4.jpg" 
      class="w-full h-full object-cover opacity-50 absolute z-10 ">

    <h1 class="text-white text-8xl font-extrabold z-0">Oizys</h1>

    <div class="z-40 w-screen mt-2">
      <MusicPlayer source="/src/assets/audio/Oizys.ogg" />
    </div>
  </div>

  <div class="bg-purple-100 flex flex-col px-12 py-24 lg:px-24 snap-start">
    <h1 
      class="text-purple-700 text-5xl lg:text-8xl font-body font-extrabold">
      Cloud dweller, <br>
      the sky is the limit.
    </h1>

    <p class="text-purple-black text-3xl lg:text-4xl font-body mt-8 leading-snug">
      Everyday I look thought the window and see the clouds. <br> <br>
      I wonder what they are thinking, what they are doing. <br> 
      I wonder if they are happy, if they are sad. <br>
      I wonder if they are free, if they are trapped. <br> 
      I wonder if they are alive, if they are dead. <br>
      I wonder if they are real, if they are fake. <br> <br>
      I wonder if they are like me, if they are like you. <br> <br>
      ☀️☀️☀️
    </p>
  </div>

  <!-- divisory -->
  <div class="bg-blue-700 h-auto p-24 text-center">
    <h1 class="text-5xl text-white font-extrabold">Soundscapes</h1>
  </div> 

  <!-- soundscapes -->
  <div class="h-[200vh] xl:flex xl:h-screen xl:w-screen xl:flex-row snap-start" id="soundscapes">
    <img 
        src="https://images2.alphacoders.com/104/1048540.jpg" 
        class="w-screen h-screen object-cover opacity-50 absolute z-10 ">
    <!-- winter -->
    <div class="bg-black w-screen xl:w-[50vw] h-screen flex flex-col justify-center items-center text-center snap-start xl:snap-none">  

      <h1 class="text-white text-8xl font-extrabold z-0">Warfare</h1>

      <div class="z-40 w-full mt-2">
        <MusicPlayer source="/src/assets/audio/Bad.wav" />
      </div>
    </div>

    <!-- dungeon -->
    <div class="bg-black w-screen xl:w-[50vw] h-screen flex flex-col justify-center items-center text-center snap-start xl:snap-none">

      <h1 class="text-white text-8xl font-extrabold z-0">Battle</h1>
      <img 
        src="https://i.pinimg.com/originals/1b/03/e0/1b03e03c6848859eeb7d18756488abce.jpg" 
        class="w-screen xl:w-[0vw] h-screen object-cover opacity-50 absolute z-10 ">

      <div class="z-40 w-full mt-2">
        <MusicPlayer source="/src/assets/audio/Gods.wav" />
      </div>
    </div>
  </div>

  <!-- sea -->
  <div class="h-[200vh] xl:flex xl:h-screen xl:w-screen xl:flex-row snap-start">
    <div class="bg-black w-screen xl:w-[50vw] h-screen flex flex-col justify-center items-center text-center">
      <img 
        src="https://images.nationalgeographic.org/image/upload/v1639146339/EducationHub/photos/pillars-of-creation.jpg" 
        class="w-screen xl:w-[50vw] h-screen object-cover opacity-50 absolute z-10 ">

      <h1 class="text-white text-8xl font-extrabold z-0">Space</h1>

      <div class="z-40 w-full mt-2">
        <MusicPlayer source="/src/assets/audio/Insolation.mp3" />
      </div>
    </div>

    <!-- wise fields -->
    <div class="bg-black w-screen xl:w-[50vw] h-screen flex flex-col justify-center items-center text-center snap-start xl:snap-none">
      <img 
        src="https://i.pinimg.com/originals/26/8c/9e/268c9e01c025c8c1a18e2450d37834d8.jpg" 
        class="w-screen xl:w-[50vw] h-screen object-cover opacity-50 absolute z-10 ">

      <h1 class="text-white text-8xl font-extrabold z-0">Wise Fields</h1>

      <div class="z-40 w-full mt-2">
        <MusicPlayer source="/src/assets/audio/Kenmeina.mp3" />
      </div>
    </div>
  </div>

  <div class="h-[200vh] xl:flex xl:h-screen xl:w-screen xl:flex-row snap-start">
    <div class="bg-black w-screen xl:w-[50vw] h-screen flex flex-col justify-center items-center text-center">
      <img 
        src="https://mdrportfolio.files.wordpress.com/2011/02/mountain-temple.jpg" 
        class="w-screen xl:w-[50vw] h-screen object-cover opacity-50 absolute z-10 ">

      <h1 class="text-white text-8xl font-extrabold z-0">Temple</h1>

      <div class="z-40 w-full mt-2">
        <MusicPlayer source="/src/assets/audio/Insolidus.mp3" />
      </div>
    </div>

    <div class="bg-black w-screen xl:w-[50vw] h-screen flex flex-col justify-center items-center text-center">
      <img 
        src="https://wallup.net/wp-content/uploads/2016/03/10/340880-fantasy_art-landscape.jpg" 
        class="w-screen xl:w-[50vw] h-full object-cover opacity-50 absolute z-10 ">

      <h1 class="text-white text-8xl font-extrabold z-0">Winter</h1>

      <div class="z-40 w-full mt-2">
        <MusicPlayer source="/src/assets/audio/Ambiance_without_perc.mp3" />
      </div>
    </div>
  </div>

  <!-- contact -->
  <div class="min-h-screen bg-blue-50 px-12 py-24 lg:px-24 flex flex-col text-center justify-center align-center" id="contact">
    <h1 class="text-blue-700 font-black text-6xl m-0 p-0 ">
      That was a ride, wasn't it?
    </h1>

    <p class="text-black font-bold text-3xl mt-4">
      I hope you enjoyed as much as I did making this website. <br>
      If you want to contact me, send me a message on Discord or an email. <br>
      I am always open to new projects and collaborations. <br>
      <span class="text-blue-600 font-black">I hope your light shines!</span> <br>
    </p>

    <div class="mt-24 mx-auto w-full flex-grow flex flex-col lg:flex-row items-center justify-center">
      <a href="https://discord.gg/km5rfvBdcZ" target="_blank" class="">
        <button 
          class="h-64 w-64 lg:h-72 lg:w-72 bg-white rounded-[2.5rem] flex flex-col items-center justify-center text-center text-xl font-bold text-[#5865F2] shadow-2xl hover:shadow-sm">
          <img src="https://assets-global.website-files.com/6257adef93867e50d84d30e2/62595384e89d1d54d704ece7_3437c10597c1526c3dbd98c737c2bcae.svg" class="w-24 h-24 m-0" />
          Join my Discord!
        </button>
      </a>

    </div>
  </div>
</div>
</template>

<script>
import MusicPlayer from './components/MusicPlayer.vue'
import Sidebar from './components/Sidebar.vue'

export default {
  components: {
    MusicPlayer, Sidebar
  }
}
</script>

<style scoped>
video {
  object-fit: cover;
  position: absolute;
  top: 0;
  left: 0;
  height: 100%;
  width: 100%;
}

.video-wrapper {
  width: 100vw;
  height: 100vh;
  position: relative;
  overflow: hidden;
  text-align: center;
  display: flex;
  align-items: center;
  justify-content: center;
}

.header {
  position: relative;
  backdrop-filter: opacity(0.5);
}

.bg-filter {
  backdrop-filter: blur(10px);
}
</style>
