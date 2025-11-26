<script setup>
// import { Link } from '@inertiajs/vue3'
// import About from '../About.vue'
// import Profile from '../Profile.vue'
// import Home from '../Home.vue'

import { ref } from 'vue'

const isMenuOpen = ref(false)

const toggleMenu = () => {
  isMenuOpen.value = !isMenuOpen.value
}

const closeMenu = () => {
  isMenuOpen.value = false
}

</script>
<template>

<div class="NavLayout">
<!-- fixed bg image -->
<div class="fixed inset-0 w-full h-full bg-center bg-no-repeat bg-cover" style="background-image: url('./images/bg9.png'); background-attachment: fixed; "></div>
<!-- Nav bar -->
    <div data-aos="fade-down" class="relative  ">
        <header class=" mt-8 fixed mx-auto max-w-6xl rounded-full left-0 right-0  bg-[#080c34]/10 backdrop-blur-md text-white text-xs p-2 max-w ">
            <nav class="flex items-center justify-between px-4">
                <div class ="logo">
                    <img src="/logo9.png" alt="logo" class ="rounded-b-sm  w-10 h-10 hover:scale-150 duration-300 cursor-pointer">
                </div>

                <aside class="hidden md:flex bg-[#253957] rounded-full text-lg font-bold space-x-8 px-8 py-1">
                    <a href="#Home" class="nav_button"> Home </a>
                    <a href="#About" class="nav_button"> About Me</a>
                    <a href="#Projects" class="nav_button"> Projects </a>
                    <a href="/My-Portfolio/Baldano_Resume.pdf" target="_blank" class="nav_button"> CV </a>
                </aside>

                <!-- hamburger design -->
                <button @click="toggleMenu" class="p-2 transition-colors rounded-full md:hidden hover:bg-white/10">

                    <div class="flex flex-col items-center justify-center w-6 h-6">
                        <span class="block w-5 h-0.5 bg-white mt-1 transition-all duration-300" :class="{ 'rotate-45 w-8 translate-y-1.5': isMenuOpen }"></span>
                        <span class="block w-5 h-0.5 bg-white mt-1 transition-all duration-100" :class="{ 'opacity-0': isMenuOpen }"></span>
                        <span class="block w-5 h-0.5 bg-white mt-1 transition-all duration-500" :class="{ '-rotate-45 -translate-y-1.5': isMenuOpen }"></span>
                    </div>
                    
                </button>
            </nav>

    <!-- Mobile Menu Overlay -->
<div v-if="isMenuOpen" class="inset-0 z-50 fixe md:hidden" @click.self="closeMenu">

  <div class=" font-bold fixed top-20 right-4 w-64 bg-[#253957]/95 backdrop-blur-md rounded-2xl shadow-xl">
    <nav class="p-6 space-y-0">
      <a href="#Home" @click="closeMenu" class="block px-4 py-3 text-white rounded-lg hover:bg-white/10">Home</a>
      <a href="#About" @click="closeMenu" class="block px-4 py-3 text-white rounded-lg hover:bg-white/10">About Me</a>
      <a href="#Projects" @click="closeMenu" class="block px-4 py-3 text-white rounded-lg hover:bg-white/10">Projects</a>
      <a href="/My-Portfolio/Baldano_Resume.pdf" target="_blank" @click="closeMenu" class="block px-4 py-3 text-white rounded-lg hover:bg-white/10">CV</a>
    </nav>
  </div>
</div>
        </header>
        <main class="p-10">
            <slot />
        </main>
    </div>
</div>

<!-- Floating Socials leftside (AI prompt)-->

<div data-aos="fade-up" class="fixed flex-col  p-2 space-y-4  -translate-y-1/2 rounded-full shadow-lg  bottom-70 left-4 ~sm/md:~mr-12/60">
  
    <!-- Facebook -->
   <a href="mailto:baldanojohnmark@gmail.com">
    <img src="https://mccedddy.github.io/portfolio/static/media/gmailDark.3253a60a2c33746c5dfb215a04f350c0.svg"
     class="socicons transition duration-300 shadow-lg  w-4.5 h-4.5 mt-1 mx-auto">
   </a>
    <a href="https://www.linkedin.com/in/john-mark-baldano-b2b69033b/" target="_blank" 
       class="p-2 transition duration-300 rounded-full shadow-lg ">
        <svg xmlns="http://www.w3.org/2000/svg" 
             class="socicons w-5 h-5 text-gray-400" fill="currentColor" viewBox="0 0 24 24">
            <path d="M20.447 20.452h-3.554V14.81c0-1.345-.027-3.078-1.877-3.078-1.88 0-2.169 1.463-2.169 2.973v5.747H9.293V9h3.415v1.561h.048c.476-.9 1.637-1.847 3.372-1.847 3.604 0 4.27 2.372 4.27 5.456v6.282zM5.337 7.433a2.062 2.062 0 1 1 0-4.125 2.062 2.062 0 0 1 0 4.125zM6.886 20.452H3.788V9h3.098v11.452z"/>
        </svg>
    </a>
    <!-- GitHub -->
  <a href="https://github.com/jmBaldano" target="_blank" 
       class="p-2 transition duration-300  rounded-full shadow-lg">
        <svg xmlns="http://www.w3.org/2000/svg" 
             class="socicons w-5 h-5 text-gray-400" fill="currentColor" viewBox="0 0 24 24">
            <path d="M12 .296a12 12 0 0 0-3.794 23.406c.6.11.82-.26.82-.577v-2.234c-3.338.727-4.042-1.61-4.042-1.61-.546-1.385-1.334-1.754-1.334-1.754-1.09-.745.083-.729.083-.729 1.205.085 1.838 1.237 1.838 1.237 1.07 1.834 2.807 1.304 3.492.997.108-.774.418-1.305.762-1.605-2.665-.304-5.466-1.334-5.466-5.931 0-1.31.469-2.38 1.236-3.221-.124-.303-.536-1.524.117-3.176 0 0 1.008-.323 3.3 1.23a11.47 11.47 0 0 1 3.003-.404c1.018.005 2.045.138 3.003.404 2.291-1.553 3.297-1.23 3.297-1.23.655 1.652.243 2.873.12 3.176.77.841 1.236 1.911 1.236 3.221 0 4.609-2.804 5.624-5.475 5.922.43.372.823 1.104.823 2.222v3.293c0 .32.216.694.826.576A12 12 0 0 0 12 .296z"/>
        </svg>
    </a>
    <!-- School  -->
    <a href="https://paraverse.feutech.edu.ph/briefcase/profile/johnmarkbaldano" target="_blank" 
       class="p-2 transition duration-300  rounded-full shadow-lg hover:scale-110 ">
        <svg xmlns="http://www.w3.org/2000/svg" 
             class="socicons w-5 h-5 text-gray-400" fill="currentColor" viewBox="0 0 24 24">
            <path d="M12 2 1 7l11 5 9-4.09V17h2V7L12 2zm0 7.75L4.21 7 12 3.25 19.79 7 12 9.75zM4 19v-6h2v6h2v-4h8v4h2v-6h2v6h2v2H2v-2h2z"/>
        </svg>
    </a>

</div>
<!-- Footer -->

<footer class="bg-white/10 backdrop-blur-md text-white text-center p-2 h-20:md items-center font-light text-sm ">
  
  <p>This website is made by John Mark Baldano. Built with VueJS and Tailwind CSS, deployed with GitHub Pages. All icons are from devicon.dev.<span class="pl-5 font-semibold">(Last Update: Nov 6, 2025)</span></p>

  
  </footer>

    
</template>