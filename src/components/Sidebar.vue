<template>
  <aside 
    @mouseenter="isHovered = true"
    @mouseleave="isHovered = false"
    class="fixed w-12 bg-transparent h-screen z-50 hover:w-64 hover:bg-black hover:bg-opacity-25 hover:backdrop-blur-xl">
      <div
        class="flex flex-col justify-center items-center h-full"
        v-if="isHovered">

        <h1 class="text-neutral-500 font-bold text-2xl">
          Menu
        </h1>

        <div class="flex flex-col justify-center  items-center">
          <a href="#home" class="text-neutral-100 font-bold text-4xl border-slate-50 mb-4 hover:text-blue-700">
            Home
          </a>
          <a href="#about" class="text-neutral-100 font-bold text-4xl border-slate-50 mb-4 hover:text-blue-700">
            About
          </a>
          <a href="#partners" class="text-neutral-100 font-bold text-4xl border-slate-50 mb-4 hover:text-blue-700">
            Partners
          </a>

          <h1 class="text-neutral-500 font-bold text-2xl">
            Projects
          </h1>
          <a href="#solo" class="text-blue-100 font-bold text-2xl border-slate-50 mb-2 hover:text-blue-700">
            Solo of the Sea
          </a>
          <a href="#record" class="text-blue-100 font-bold text-2xl border-slate-50 mb-2 hover:text-blue-700">
            For the Record
          </a>
          <a href="#angels" class="text-blue-100 font-bold text-2xl border-slate-50 mb-2 hover:text-blue-700">
            Angels
          </a>
          <a href="#undead-commander" class="text-blue-100 font-bold text-2xl border-slate-50 mb-2 hover:text-blue-700">
            Commander
          </a>
          <a href="#awoken" class="text-blue-100 font-bold text-2xl border-slate-50 mb-2 hover:text-blue-700">
            Awoken
          </a>
          <a href="#soundscapes" class="text-blue-100 font-bold text-2xl border-slate-50 mb-2 hover:text-blue-700">
            Soundscapes
          </a>

          <h1 class="text-neutral-500 font-bold text-2xl">
            Finally
          </h1>
          <a href="#contact" class="text-neutral-100 font-bold text-4xl border-slate-50 mb-4 hover:text-blue-700">
            Contact
          </a>
        </div>
      </div>
  </aside>
</template>

<script>
export default {
  name: 'Scrollbar',
  data() {
    return {
      isHovered: false
    }
  },
}
</script>

<style scoped>
ul {
  list-style-type: none;
}
</style>