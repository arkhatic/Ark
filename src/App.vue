<template>
  <Sidebar />
  <!-- landing page -->
  <div class="bg-black h-screen" id="home">
    <div class="flex flex-col justify-center h-full text-left mx-24">
      <h1 class="text-9xl text-blue-600 font-extrabold">
        Arkhatic, 
      </h1>

      <h1 class="text-6xl text-white font-extrabold">
        award-winning <br>
        composer and scorer.
      </h1>

      <a href="https://linktree.com/arkhatic" class="mt-4 text-xl text-blue-600 font-extrabold">@arkhatic</a>
    </div>
  </div>

  <!-- about page -->
  <div class="bg-white h-auto p-24" id="about">
    <div class="flex flex-col text-left">
      <h1 class="text-8xl text-black font-extrabold">
        I have been always learning alone.
      </h1>
      
      <div class="flex flex-row mt-4">
        <p class="text-3xl text-black font-bold mt-4">
          Nothing is easy. <br> <br>
          
          Years ago, I decided to study music, without having a tip of how difficult it really is. Without any support from my parents, I kept pressing on even when the times hardened out quite a lot. <br> <br>

          When I got my first job as a composer, I felt, for the first time, <br> 
          <span class="text-blue-800">a glance of happiness</span>.<br>

          So that is me, a ship who doens't stop sailing, even when the sea is rough. <br> <br>
          In other words, an <span class="text-blue-800">ark</span>.
        </p>
      </div>
    </div>  
  </div>  

  <!-- partners page -->
  <div class="min-h-screen bg-green-100 p-24 flex flex-col" id="partners">
    <div>
      <h1 class="text-7xl text-green-700 font-black">Fortunately, I don't work alone anymore.</h1>

      <h2 class="text-4xl text-black font-extrabold mt-4">
        A <span class="text-green-600 text-5xl">huge</span> thanks to the guys below for helping me get into places I did not know were possible to reach and to overcome the challenges of every day. ❤️
      </h2>
    </div>

    <div class="flex h-full flex-grow flex-col justify-center items-center">
      <div class="h-full grid grid-cols-3 grid-rows-1 gap-12 items-center justify-center">
        <a href="https://pesadelum.com">
          <img 
            class="w-full filter grayscale hover:grayscale-0 rounded-xl"
            src="https://cdn.discordapp.com/attachments/853715361568129054/1033771155590484088/PESADELUM_2.webp" />
        </a>

        <a href="https://wonderacid-studio.vercel.app">
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
    <h1 class="text-7xl text-white font-extrabold">Let us look at some of <span class="italic">my</span> projects.</h1>
  </div> 

  <!-- the undead commander -->
  <div class="bg-black h-screen flex flex-col justify-center items-center text-center" id="undead-commander">
    <img 
      src="https://cdn.cnn.com/cnnnext/dam/assets/140828132531-01-world-war-ii-0828.jpg" 
      class="w-full h-full object-cover opacity-50 absolute z-10 ">

    <h1 class="text-white text-8xl font-extrabold z-0">The Undead Commander</h1>

    <div class="z-40 w-screen mt-2">
      <MusicPlayer source="https://cdn.discordapp.com/attachments/853715361568129054/1033707650355048458/Marta.wav" />
    </div>
  </div>

  <div class="bg-black flex flex-col p-24">
    <h1 
      class="text-white text-7xl font-details text-center">
      In modern warfare, there are no victors; <br> 
      there are only survivors.
    </h1>

    <p class="text-white text-4xl font-details text-center mt-8">
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
  <div class="bg-black h-screen flex flex-col justify-center items-center text-center" id="awoken">
    <img 
      src="https://r4.wallpaperflare.com/wallpaper/432/899/621/fantasy-art-clouds-digital-art-futuristic-wallpaper-8d1bdf2ceb7791f3e2be17e2500dcba4.jpg" 
      class="w-full h-full object-cover opacity-50 absolute z-10 ">

    <h1 class="text-white text-8xl font-extrabold z-0">Awoken</h1>

    <div class="z-40 w-screen mt-2">
      <MusicPlayer source="https://cdn.discordapp.com/attachments/853715361568129054/1033707228588425236/Cantus_of_Requiem.mp3" />
    </div>
  </div>

  <div class="bg-purple-100 flex flex-col p-24">
    <h1 
      class="text-purple-700 text-7xl font-display font-black">
      Clouds dwelings, <br>
      the sky is the limit.
    </h1>

    <p class="text-purple-black text-4xl font-details mt-8">
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
  <div class="bg-orange-700 h-auto p-24 text-center">
    <h1 class="text-7xl text-white font-extrabold">Soundscapes ahead!</h1>
  </div> 

  <!-- winter -->
  <div class="flex h-screen w-screen flex-rows" id="soundscapes">
    <div class="bg-black w-[50vw] h-screen flex flex-col justify-center items-center text-center">
      <img 
        src="https://wallup.net/wp-content/uploads/2016/03/10/340880-fantasy_art-landscape.jpg" 
        class="w-[50vw] h-full object-cover opacity-50 absolute z-10 ">

      <h1 class="text-white text-8xl font-extrabold z-0">Winter</h1>

      <div class="z-40 w-full mt-2">
        <MusicPlayer source="https://cdn.discordapp.com/attachments/853715361568129054/1033787829228150925/Ambiance_without_perc.mp3" />
      </div>
    </div>

    <div class="bg-black w-[50vw] h-full flex flex-col justify-center items-center text-center">
      <img 
        src="https://images4.alphacoders.com/283/283686.jpg" 
        class="w-[50vw] h-full object-cover opacity-50 absolute z-10 ">

      <h1 class="text-white text-8xl font-extrabold z-0">Dungeon</h1>

      <div class="z-40 w-full mt-2">
        <MusicPlayer source="https://cdn.discordapp.com/attachments/853715361568129054/1033793622321135626/Solo_of_the_Sea.wav" />
      </div>
    </div>
  </div>

  <div class="flex h-screen w-screen flex-rows">
    <div class="bg-black w-[50vw] h-screen flex flex-col justify-center items-center text-center">
      <img 
        src="https://cdn.wallpapersafari.com/0/62/1PULhg.jpg" 
        class="w-[50vw] h-full object-cover opacity-50 absolute z-10 ">

      <h1 class="text-white text-8xl font-extrabold z-0">Sea</h1>

      <div class="z-40 w-full mt-2">
        <MusicPlayer source="https://cdn.discordapp.com/attachments/853715361568129054/1033798112671707206/Epic_but_Gentle.wav" />
      </div>
    </div>

    <div class="bg-black w-[50vw] h-full flex flex-col justify-center items-center text-center">
      <img 
        src="https://i.pinimg.com/originals/26/8c/9e/268c9e01c025c8c1a18e2450d37834d8.jpg" 
        class="w-[50vw] h-full object-cover opacity-50 absolute z-10 ">

      <h1 class="text-white text-8xl font-extrabold z-0">Wise Fields</h1>

      <div class="z-40 w-full mt-2">
        <MusicPlayer source="https://cdn.discordapp.com/attachments/853715361568129054/1033793736817266770/Kenmeina_bunya.wav" />
      </div>
    </div>
  </div>

  <div class="min-h-screen bg-blue-50 p-24 flex flex-col text-center justify-center align-center" id="contact">
    <h1 class="text-blue-700 font-black text-8xl m-0 p-0 ">
      That was a ride, wasn't it?
    </h1>

    <p class="text-black font-bold text-4xl mt-4">
      I hope you enjoyed as much as I did making this website. <br>
      If you want to contact me, send me a message on Discord or an email. <br>
      I am always open to new projects and collaborations. <br>
      <span class="text-blue-600 font-black">I hope your light shines!</span> <br>
    </p>

    <div class="mt-24 mx-auto sm:w-full md:w-full lg:w-4/6 2xl:w-1/2 flex-grow flex flex-row items-center justify-between">
      <a href="https://discord.gg/km5rfvBdcZ" target="_blank" class="">
        <button 
          class="h-72 w-72 bg-white rounded-[2.5rem] flex flex-col items-center justify-center text-center text-xl font-bold text-[#5865F2] shadow-2xl hover:shadow-sm">
          <img src="https://assets-global.website-files.com/6257adef93867e50d84d30e2/62595384e89d1d54d704ece7_3437c10597c1526c3dbd98c737c2bcae.svg" class="w-24 h-24 m-0" />
          Join my Discord!
        </button>
      </a>

      <div class="w-2 h-96 bg-[#5865F2]"></div>

      <a href="mailto:arkhatic.sousa@gmail.com" target="_blank" class="">
        <button 
          class="h-72 w-72 bg-white rounded-[2.5rem] flex flex-col items-center justify-center text-center text-xl font-bold text-[#5865F2] shadow-2xl hover:shadow-sm">
          <img src="https://cdn.discordapp.com/attachments/853715361568129054/1033805220553175050/free-mail-icon-142-thumb.png" class="w-24 h-24 m-0" />
          Send me an email!
        </button>
      </a>
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

