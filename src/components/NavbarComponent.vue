<template>
  <nav class="w-full text-white flex justify-between p-4">
    <router-link to="/" class="">Porfolio</router-link>
    <ul class="flex gap-10">
      <li>
        <router-link to="/" class="hover:underline hover:text-teal-400"><span class="text-teal-400">1. </span>Home</router-link>
      </li>
      <li>
        <router-link to="/about" class="hover:underline hover:text-teal-400"><span class="text-teal-400">2. </span>Sobre</router-link>
      </li>
      <li>
        <router-link to="/projects" class="hover:underline hover:text-teal-400"><span class="text-teal-400">3. </span>Projetos</router-link
        >
      </li>
      <li>
        <router-link to="/contacts" class="hover:underline hover:text-teal-400"
          ><span class="text-teal-400">4. </span>Contato</router-link
        >
      </li>
    </ul>
  </nav>
</template>
