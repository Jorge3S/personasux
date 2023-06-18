<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <nav class="flex items-center bg-blue-600 p-3 flex-wrap">
    <a href="#" class="p-2 mr-4 inline-flex items-center">

      <span class="text-xl text-black font-bold uppercase tracking-wide">Programación Web II</span>
    </a>
    <button
      class="text-black inline-flex p-3 hover:bg-gray-700 rounded lg:hidden ml-auto hover:text-gray outline-none nav-toggler"
      data-target="#navigation">
      <i class="material-icons">
        MENÚ
      </i>
    </button>
    <div class="hidden top-navbar w-full lg:inline-flex lg:flex-grow lg:w-auto" id="navigation">
      <div
        class="lg:inline-flex lg:flex-row lg:ml-auto lg:w-auto w-full lg:items-center items-start  flex flex-col lg:h-auto">
        <a href="#"
          class="lg:inline-flex lg:w-auto w-full px-3 py-2 rounded text-black-400 items-center justify-center hover:bg-gray-900 hover:text-white">
          <span>
            <RouterLink to="/">Inicio</RouterLink>
          </span>
        </a>
        <a href="#"
          class="lg:inline-flex lg:w-auto w-full px-3 py-2 rounded text-black-400 items-center justify-center hover:bg-gray-900 hover:text-white">
          <span>
            <RouterLink to="/about">Registrarse</RouterLink>
          </span>
        </a>
        <a href="#"
          class="lg:inline-flex lg:w-auto w-full px-3 py-2 rounded text-black-400 items-center justify-center hover:bg-gray-900 hover:text-white">
          <span>
            <RouterLink to="/mostrar" class="py-5">Ver registros</RouterLink>
          </span>
        </a>

      </div>
    </div>
  </nav>
  <RouterView />
</template>