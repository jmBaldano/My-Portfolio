<template>
    <div class="sections">
        <h1 class="title py-10 text-5xl font-bold text-center">
            PROJECTS
        </h1>
        <!-- Coserve -->
        <div class="flex flex-col items-center md:flex-row gap-20 mt-10 px-4">
            <div class="w-full md:w-[63%]">
                <img src="/images/coserve1.png" alt="Coserve" class="hover rounded-lg shadow-lg">
            </div>

            <div class="hover ml-10 md:w-1/2 rounded-lg shadow-lg">
                <h2 class="header leading-relaxed">
                    Coserve
                </h2>
                <p class="desc">
                    A Web Barangay Property Reservation with Billing System and Financial Analytics for Brgy. Batasan Hills
                </p>
                 <!-- stack used -->
            <div class=" flex flex-row gap-4">
                <div class="mt-6 ">
                    <a href="https://laravel.com/" target="blank">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/laravel/laravel-original.svg" 
                    alt="vuejs" 
                    class="stack-used w-7 h-7 hover:scale-150 duration-300 cursor-pointer" />
                    </a>
                </div>
                <div class="mt-6 ">
                    <a href="https://tailwindcss.com/" target="blank">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/tailwindcss/tailwindcss-original.svg" 
                    alt="tailwindcss" 
                    class="stack-used w-7 h-7 hover:scale-150 duration-300 cursor-pointer" />
                    </a>
                </div>
                <div class="mt-6 ">
                    <a href="https://figma.com/" target="blank">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/figma/figma-original.svg" 
                    alt="tailwindcss" 
                    class="stack-used w-7 h-7 hover:scale-150 duration-300 cursor-pointer" />
                    </a>
                </div>
            </div>
            </div>
        </div>


        <!-- Gamehaven -->
        <div class="flex flex-col items-center md:flex-row gap-20 mt-10 px-4">
           
            <div class="w-full md:w-[70%]">
                <img 
                    src="/images/gamehaven1.png" 
                    alt="Game Haven Project" 
                    class="hover rounded-lg shadow-lg cursor-pointer" @click="open=true" >
            </div>
            
            
            <!-- Right Description -->
            <div class="hover w-full m-10 md:w-1/2 rounded-lg shadow-lg">
                <h2 class="header mb-4 text-3xl font-bold text-white">Game Haven</h2>
                <p class="desc text-lg leading-relaxed">
                    E-commerce platform designed for gamers, 
                    offering a wide range of  gaming consoles and other gaming accessories
                </p>
                 <!-- stack used -->
                <div class="mt-6 ">
                    <a href="https://www.odoo.com/slides/slide/website-configurator-6929" target="blank">
                    <img src="https://mccedddy.github.io/portfolio/static/media/odoo.d7269ac577bab53a792aeadffe735964.svg" 
                    alt="odoo" 
                    class="stack-used w-7 h-7 hover:scale-150 duration-300 cursor-pointer" />
                    </a>
                </div>
            </div >
            <!--gamehaven modal -->
            <!-- <div v-if="open" class="fixed inset-0 bg-black/85 flex justify-center items-center z-1 " @click="open=false">
                <div class="relative ">
                    <div ref="container" class="relative  max-w-3xl  right-50 bg-white/50 overflow-hidden rounded-lg shadow-lg gap-10" @click.stop>
                        <div ref="carousel" class="flex transition-transform duration-300">
                            <img src="/images/gamehaven2.png" alt="gamehaven1" class="w-full">
                            <img src="/images/gamehaven3.png" alt="gamehaven2" class="w-full">
                            <img src="/images/gamehaven4.png" alt="gamehaven3" class="w-full">
                            <img src="/images/gamehaven5.png" alt="gamehaven4" class="w-full">
                        </div>
                        <button @click="prevSlide" class="text-3xl absolute top-1/2 left-2 -translate-y-1/2 bg-black/50 text-white p-2 rounded-full cursor-pointer">❮</button>
                        <button @click="nextSlide" class="text-3xl absolute top-1/2 right-2 -translate-y-1/2 bg-black/50 text-white p-2 rounded-full cursor-pointer">❯</button>
                    </div>
                </div>
               
                    <p class="text-white text-3xl ">
                        Desc
                    </p>
               
            </div> -->
                

        </div>

<!-- Portfolio proj -->
        <div class="flex flex-col items-center md:flex-row gap-20 mt-10 px-4">
           
            <div class="w-full md:w-[70%]">
                <img 
                    src="/images/portfolio.png" 
                    alt="Portfolio" 
                    class="hover rounded-lg shadow-lg" >
            </div>
            
            
            <!-- Right Description -->
            <div class="hover w-full m-10 md:w-1/2 rounded-lg shadow-lg">
                <h2 class="header mb-4 text-3xl font-bold text-white">Personal Portfolio</h2>
                <p class="desc text-lg leading-relaxed">
                   This is my portfolio website, where I showcase my Experience througout my journey as a developer.
                </p>
                <!-- stack used -->
                <div class="mt-6 flex flex-row space-x-3">
                    
                    <a href="https://www.vuejs.org" target="blank">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/vuejs/vuejs-original.svg" 
                    alt="vuejs" 
                    class="stack-used w-7 h-7 hover:scale-150 duration-300 cursor-pointer" />
                    </a>
                    
                    
                     <a href="https://www.tailwindcss.com" target="blank">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/tailwindcss/tailwindcss-original.svg" 
                    alt="tailwindcss" 
                    class="stack-used w-7 h-7 hover:scale-150 duration-300 cursor-pointer" />
                    </a>
                    
                </div>
                
            </div>
        </div>
<!-- Rock, Paper, Scissors proj-->
        <div class="flex flex-col items-center md:flex-row gap-20 mt-10 px-4">
           
            <div class="w-full md:w-[70%]">
                <img 
                    src="/images/rps1.png" 
                    alt="Portfolio" 
                    class="hover rounded-lg shadow-lg" >
            </div>
            
            
            <!-- Right Description -->
            <div class="hover w-full m-10 md:w-1/2 rounded-lg shadow-lg">
                <h2 class="header mb-4 text-3xl font-bold text-white">Rock, Paper, Scissors</h2>
                <p class="desc text-lg leading-relaxed">
                   A simple minigame project for rock paper and scissors
                   <br>
                   Visit:
                   <a href="https://jmbaldano.github.io/Rock-Paper-and-Scissors/" target="_blank" class="hover:scale-110 transform transition duration-300 hover:underline">
                    Rock, Paper, Scissors
                    </a>
                    
                </p>
                
                <!-- stack used -->
                <div class="mt-6 flex flex-row space-x-3">
                    
                    <a href="https://www.vuejs.org" target="blank">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/html5/html5-original.svg" 
                    alt="html5" 
                    class="stack-used w-7 h-7 hover:scale-150 duration-300 cursor-pointer" />
                    </a>
                    
                    
                     <a href="https://www.tailwindcss.com" target="blank">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/css3/css3-original.svg" 
                    alt="css3" 
                    class="stack-used w-7 h-7 hover:scale-150 duration-300 cursor-pointer" />
                    </a>

                     <a href="https://www.tailwindcss.com" target="blank">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/javascript/javascript-original.svg" 
                    alt="js" 
                    class="stack-used w-7 h-7 hover:scale-150 duration-300 cursor-pointer" />
                    </a>
                    
                </div>
                
            </div>
        </div>

        <!-- Real Estate Website -->
        <div class="flex flex-col items-center md:flex-row gap-20 mt-10 px-4">
           
            <div class="w-full md:w-[70%]">
                <img 
                    src="/images/realEstate1.png" 
                    alt="Portfolio" 
                    class="hover rounded-lg shadow-lg" >
            </div>
            
            
            <!-- Right Description -->
            <div class="hover w-full m-10 md:w-1/2 rounded-lg shadow-lg">
                <h2 class="header mb-4 text-3xl font-bold text-white">Real Estate Website</h2>
                <p class="desc text-lg leading-relaxed">
                   A Real estate personal website
                   <br>
                   Visit:
                   <a href="https://real-estate-website-five-mu.vercel.app/" target="_blank" class="hover:scale-110 transform transition duration-300 hover:underline">
                    Real Estate Website
                    </a>
                </p>
                
                <!-- stack used -->
               <div class="mt-6 flex flex-row space-x-3">
                    
                    <a href="https://www.vuejs.org" target="blank">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/vuejs/vuejs-original.svg" 
                    alt="vuejs" 
                    class="stack-used w-7 h-7 hover:scale-150 duration-300 cursor-pointer" />
                    </a>
                    
                    
                     <a href="https://www.tailwindcss.com" target="blank">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/tailwindcss/tailwindcss-original.svg" 
                    alt="tailwindcss" 
                    class="stack-used w-7 h-7 hover:scale-150 duration-300 cursor-pointer" />
                    </a>
                    
                </div>
            </div>
        </div>
        <!-- Portfolio Website -->
        <div class="flex flex-col items-center md:flex-row gap-20 mt-10 px-4">
           
            <div class="w-full md:w-[70%]">
                <img 
                    src="/images/mhelPortfolio1.png" 
                    alt="Portfolio" 
                    class="hover rounded-lg shadow-lg" >
            </div>
            
            
            <!-- Right Description -->
            <div class="hover w-full m-10 md:w-1/2 rounded-lg shadow-lg">
                <h2 class="header mb-4 text-3xl font-bold text-white">Portfolio Website</h2>
                <p class="desc text-lg leading-relaxed">
                   A Personal portfolio website
                   <br>
                   Visit:
                   <a href="https://mhel-portfolio.vercel.app/" target="_blank" class="hover:scale-110 transform transition duration-300 hover:underline">
                    Portfolio Website
                    </a>
                </p>
                
                <!-- stack used -->
               <div class="mt-6 flex flex-row space-x-3">
                    
                    <a href="https://www.vuejs.org" target="blank">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/vuejs/vuejs-original.svg" 
                    alt="vuejs" 
                    class="stack-used w-7 h-7 hover:scale-150 duration-300 cursor-pointer" />
                    </a>
                    
                    
                     <a href="https://www.tailwindcss.com" target="blank">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/tailwindcss/tailwindcss-original.svg" 
                    alt="tailwindcss" 
                    class="stack-used w-7 h-7 hover:scale-150 duration-300 cursor-pointer" />
                    </a>
                    
                </div>
            </div>
        </div>

    </div>

</template>
<script setup>
 import {ref, onMounted, onBeforeUnmount} from "vue";
 const open =ref(false);
 const carousel = ref(null);
 const container = ref(null);
 const index = ref(0);
 
const totalSlides = 4;

function slideWidth() {
  return container.value ? container.value.clientWidth : 0;
}

function showSlide() {
  if (carousel.value) {
    carousel.value.style.transform = `translateX(-${index.value * slideWidth()}px)`;
  }
}

function nextSlide() {
  index.value = (index.value + 1) % totalSlides;
  showSlide();
}

function prevSlide() {
  index.value = (index.value - 1 + totalSlides) % totalSlides;
  showSlide();
}

</script>




