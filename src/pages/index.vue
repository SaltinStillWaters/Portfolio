<template>
  <About />
  <Projects @onClick="projectClick"/>
  <ProjectOverlay :open-overlay="openOverlay", :project-id="projectId" @closed="openOverlay=false"/>
  <Experience />
  <Resume />
  <Contact />
</template>

<script setup>
import { ref } from 'vue';

  const projectId = ref(0);
  const openOverlay = ref(false);

  function projectClick(i) {
    openOverlay.value = true;
    projectId.value = i
  }
</script>
