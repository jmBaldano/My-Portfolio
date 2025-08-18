<script setup>
import { ref } from 'vue'

</script>
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
                    class="hover rounded-lg shadow-lg" >
            </div>
            
            
            <!-- Right Description -->
            <div class="hover w-full m-10 md:w-1/2 rounded-lg shadow-lg">
                <h2 class="header mb-4 text-3xl font-bold text-white">Game Haven</h2>
                <p class="desc text-lg leading-relaxed">
                    E-commerce platform designed for gamers, 
                    offering a wide range of  gaming consoles and other gaming accessories
                </p>
                <div class="mt-6 ">
                    <a href="https://www.odoo.com/slides/slide/website-configurator-6929" target="blank">
                    <img src="https://mccedddy.github.io/portfolio/static/media/odoo.d7269ac577bab53a792aeadffe735964.svg" 
                    alt="odoo" 
                    class="stack-used w-7 h-7 hover:scale-150 duration-300 cursor-pointer" />
                    </a>
                </div>
            </div>
        </div>

        <div class="flex flex-col items-center md:flex-row gap-20 mt-10 px-4">
           
            <div class="w-full md:w-[70%]">
                <img 
                    src="/images/portfolio.png" 
                    alt="Game Haven Project" 
                    class="hover rounded-lg shadow-lg" >
            </div>
            
            
            <!-- Right Description -->
            <div class="hover w-full m-10 md:w-1/2 rounded-lg shadow-lg">
                <h2 class="header mb-4 text-3xl font-bold text-white">Personal Portfolio</h2>
                <p class="desc text-lg leading-relaxed">
                   This is my portfolio website, where I showcase my Experience througout my journey as a developer.
                </p>
                <div class="mt-6 flex flex-row space-x-3">
                    
                    <a href="https://www.vuejs.org" target="blank">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/vuejs/vuejs-original.svg" 
                    alt="odoo" 
                    class="stack-used w-7 h-7 hover:scale-150 duration-300 cursor-pointer" />
                    </a>
                    
                    
                     <a href="https://www.tailwindcss.com" target="blank">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/tailwindcss/tailwindcss-original.svg" 
                    alt="odoo" 
                    class="stack-used w-7 h-7 hover:scale-150 duration-300 cursor-pointer" />
                    </a>
                    
                </div>
                
            </div>
        </div>

    </div>
</template>




