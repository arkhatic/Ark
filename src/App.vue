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

  <div class="bg-black h-auto p-12 lg:p-24 w-screen" id="award">
    <h1 class="text-5xl lg:text-6xl xl:text-7xl text-white font-black font-display">Also, in 2022, I won the Hacelo Corto award for the best film score!</h1>
    <h2 class="text-2xl text-white font-bold mt-4 max-w-full">Hacelo Corto is a festival of short films hosted in Buenos Aires, Argentina. <br>
    Our film, Sonitus, won the award for the best score and special mention of the Jury, for its creative drama and emotive all-out soundtrack. <br>
    But, it would not be possible without the help of my team 💖 </h2>

    <h1 class="text-3xl text-black font-black text-white my-3">Hear the OST below!</h1>
    <div class="bg-black py-10 flex flex-col justify-center items-center text-center rounded-xl bg-yelllow-600">
      <h1 class="text-white px-12 text-4xl lg:text-4xl font-extrabold z-0">Sonitus</h1>

      <div class="z-40 w-screen mt-2">
        <MusicPlayer source="https://cdn.discordapp.com/attachments/1146403851352682636/1146406420263211049/01_-_Unknown_Artist_-_Duet_unmixed.mp3" />
      </div>
    </div>

  </div>

  <!-- partners page -->
  <div class="min-h-screen bg-green-100 p-12 lg:p-24 flex flex-col" id="partners">
    <div>
      <h1 class="text-5xl lg:text-6xl xl:text-7xl text-green-700 font-black font-display">Fortunately, I don't work alone anymore.</h1>

      <h2 class="text-3xl text-black font-extrabold mt-8 lg:mt-4">
        A <span class="text-green-600 text-4xl">huge</span> thanks to the guys below for helping me get into places I did not know were possible to reach and to overcome the challenges of every day. ❤️
      </h2>
    </div>

    <div class="flex h-full flex-grow flex-col justify-center items-center">
      <div class="h-full mt-8 grid grid-cols-1 grid-rows-3 px-0 md:px-24 lg:mt-0 lg:p-0 lg:grid-cols-3 lg:grid-rows-1 gap-8 lg:gap-12 items-center justify-center">
        <a href="https://pesadelum.com">
          <img 
            class="w-full filter grayscale hover:grayscale-0 rounded-xl"
            src="https://cdn.discordapp.com/attachments/853715361568129054/1033771155590484088/PESADELUM_2.webp" />
        </a>

        <a href="https://wonderacid.web.app">
          <img 
            class="w-full filter grayscale hover:grayscale-0 rounded-xl"
            src="https://cdn.discordapp.com/attachments/853715361568129054/1033771276206100581/logo-squared.png" />
        </a>

        <a href="https://watashipx.com/raifuejji">
          <img 
            class="w-full filter grayscale hover:grayscale-0 rounded-xl"
            src="https://cdn.discordapp.com/attachments/853715361568129054/1033771310158987416/sky_raiders.png" />
        </a>
      </div>
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
      <MusicPlayer source="https://cdn.discordapp.com/attachments/1117080918344093796/1117080918708985896/01_-_Arkhatic_-_Solo_of_the_Sea_-_Orchestra.mp3" />
    </div>
  </div>

  <div class="bg-black h-screen flex flex-col justify-center items-center text-center snap-start" id="record">
    <img 
      src="https://cutewallpaper.org/21/fantasy-hd-wallpaper/Fantasy-Art-Wallpapers-HD-PixelsTalkNet.jpg" 
      class="w-full h-full object-cover opacity-50 absolute z-10 ">

    <h1 class="text-white px-12 text-6xl lg:text-8xl font-extrabold z-0">For the Record</h1>

    <div class="z-40 w-screen mt-2">
      <MusicPlayer source="https://cdn.discordapp.com/attachments/1153341833942937621/1153341835389964389/01_-_Arkhatic_-_For_the_Record.mp3" />
    </div>
  </div>

  <div class="bg-black h-screen flex flex-col justify-center items-center text-center snap-start" id="angels">
    <img 
      src="https://cdn.discordapp.com/attachments/1146407169508515870/1146407258721370193/4586501-fantasy-art-fantasy-city-war-battle.jpg" 
      class="w-full h-full object-cover opacity-50 absolute z-10 ">

    <h1 class="text-white px-12 text-6xl lg:text-8xl font-extrabold z-0">Angels</h1>

    <div class="z-40 w-screen mt-2">
      <MusicPlayer source="https://cdn.discordapp.com/attachments/1116890333071028264/1116890333393977455/Angels.mp3" />
    </div>
  </div>

  <!-- the undead commander -->
  <div class="bg-black h-screen flex flex-col justify-center items-center text-center snap-start" id="undead-commander">
    <img 
      src="https://cdn.cnn.com/cnnnext/dam/assets/140828132531-01-world-war-ii-0828.jpg" 
      class="w-full h-full object-cover opacity-50 absolute z-10 ">

    <h1 class="text-white px-12 text-6xl lg:text-8xl font-extrabold z-0">The Undead Commander</h1>

    <div class="z-40 w-screen mt-2">
      <MusicPlayer source="https://cdn.discordapp.com/attachments/853715361568129054/1033707650355048458/Marta.wav" />
    </div>
  </div>

  <div class="bg-black flex flex-col px-12 py-24 lg:px-24 snap-start">
    <h1 
      class="text-white text-5xl lg:text-7xl font-details text-center">
      In modern warfare, there are no victors; <br> 
      there are only survivors.
    </h1>

    <p class="text-white text-3xl lg:text-4xl font-details text-center mt-8 leading-snug">
      When I am composing a song, I like to imagine a story behind it. <br> <br>
      This is the story of a commander who was killed in the battlefield, but was brought back to life.<br>
      Even dead, the soldier's only thoughts are of protecting home, <br>
      and his squad will do <span class="text-red-500">anything</span> to achieve that goal. <br>
    </p>

    <p class="text-white text-4xl font-details text-center mt-8">
      That is how this <span class="text-yellow-300">majestic</span> and <span class="text-blue-600">sorrow</span> song was born.
    </p>
  </div>

  <!-- cantus of requiem -->
  <div class="bg-black h-screen flex flex-col justify-center items-center text-center snap-start" id="awoken">
    <img 
      src="https://r4.wallpaperflare.com/wallpaper/432/899/621/fantasy-art-clouds-digital-art-futuristic-wallpaper-8d1bdf2ceb7791f3e2be17e2500dcba4.jpg" 
      class="w-full h-full object-cover opacity-50 absolute z-10 ">

    <h1 class="text-white text-8xl font-extrabold z-0">Awoken</h1>

    <div class="z-40 w-screen mt-2">
      <MusicPlayer source="https://cdn.discordapp.com/attachments/853715361568129054/1033707228588425236/Cantus_of_Requiem.mp3" />
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
        src="https://cdn.discordapp.com/attachments/1146407169508515870/1146407451294433351/140887-fantasy-art-spear-medieval-castle.jpg" 
        class="w-screen h-screen object-cover opacity-50 absolute z-10 ">
    <!-- winter -->
    <div class="bg-black w-screen xl:w-[50vw] h-screen flex flex-col justify-center items-center text-center snap-start xl:snap-none">  

      <h1 class="text-white text-8xl font-extrabold z-0">Warfare</h1>

      <div class="z-40 w-full mt-2">
        <MusicPlayer source="https://cdn.discordapp.com/attachments/1146408667235754005/1146408667877486632/Mixdown_1.mp3" />
      </div>
    </div>

    <!-- dungeon -->
    <div class="bg-black w-screen xl:w-[50vw] h-screen flex flex-col justify-center items-center text-center snap-start xl:snap-none">

      <h1 class="text-white text-8xl font-extrabold z-0">Battle</h1>
      <img 
        src="https://i.pinimg.com/originals/1b/03/e0/1b03e03c6848859eeb7d18756488abce.jpg" 
        class="w-screen xl:w-[0vw] h-screen object-cover opacity-50 absolute z-10 ">

      <div class="z-40 w-full mt-2">
        <MusicPlayer source="https://cdn.discordapp.com/attachments/1146408536155365498/1146408536876789831/Gods_Plugged.mp3" />
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
        <MusicPlayer source="https://cdn.discordapp.com/attachments/1146410086546296832/1146410086940545097/Insolation.mp3" />
      </div>
    </div>

    <!-- wise fields -->
    <div class="bg-black w-screen xl:w-[50vw] h-screen flex flex-col justify-center items-center text-center snap-start xl:snap-none">
      <img 
        src="https://i.pinimg.com/originals/26/8c/9e/268c9e01c025c8c1a18e2450d37834d8.jpg" 
        class="w-screen xl:w-[50vw] h-screen object-cover opacity-50 absolute z-10 ">

      <h1 class="text-white text-8xl font-extrabold z-0">Wise Fields</h1>

      <div class="z-40 w-full mt-2">
        <MusicPlayer source="https://cdn.discordapp.com/attachments/1146409704491327488/1146409704839462962/01_-_Unknown_Artist_-_Kenmeina_bunya.mp3" />
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
        <MusicPlayer source="https://cdn.discordapp.com/attachments/1146409302500851742/1146409303142576168/Insolidus.mp3" />
      </div>
    </div>

    <div class="bg-black w-screen xl:w-[50vw] h-screen flex flex-col justify-center items-center text-center">
      <img 
        src="https://wallup.net/wp-content/uploads/2016/03/10/340880-fantasy_art-landscape.jpg" 
        class="w-screen xl:w-[50vw] h-full object-cover opacity-50 absolute z-10 ">

      <h1 class="text-white text-8xl font-extrabold z-0">Winter</h1>

      <div class="z-40 w-full mt-2">
        <MusicPlayer source="https://cdn.discordapp.com/attachments/853715361568129054/1033787829228150925/Ambiance_without_perc.mp3" />
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
