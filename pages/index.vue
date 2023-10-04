<template>
  <section>
    <div class="grid md:grid-cols-2">
      <div class="flex flex-col py-4 justify-around">
        <div class="flex flex-col gap-4">
          <h2>Bienvenue sur mon blog</h2>
          <p class="text-xl">
            Tu retrouveras ici les dernières actualitées de mes projets ainsi que des articles sur les différentes
            technologies utilisé au cours de ceux-ci !
          </p>
        </div>
        <div class="flex flex-col gap-4">
          <h3>Inscris toi à la newsletter pour suivre mon actualité !</h3>
          <input type="email" placeholder="Adresse mail"
                 class="bg-theme-01 border-2 border-theme-02 rounded-md p-2 w-1/2">
        </div>
      </div>
      <NuxtImg src="/hero-img.png"/>
    </div>
  </section>
  <section>
    <h2>Projet en cours</h2>
    <ContentList path="/projects" v-slot="{ list }">
      <div v-for="projects in list" :key="projects._path">
        <NuxtImg :src="projects.image" class="h-48 w-96 object-cover rounded-t-md"/>
        {{projects.title}}
      </div>
    </ContentList>
  </section>
</template>
<script setup>
</script>