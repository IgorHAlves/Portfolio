<template>
  <nav class="w-full bg-teal-900 text-white flex justify-between p-4">
    <span class="">Porfolio</span>
    <ul class="flex gap-10">
      <li>
        <router-link to="/home" class="hover:underline">Home</router-link>
      </li>
      <li>
        <router-link to="/about" class="hover:underline">Sobre</router-link>
      </li>
      <li>
        <router-link to="/projects" class="hover:underline"
          >Projetos</router-link
        >
      </li>
      <li>
        <router-link to="/contacts" class="hover:underline"
          >Contato</router-link
        >
      </li>
    </ul>
  </nav>
</template>
