<script setup lang="ts">
import Card from 'primevue/card';

const props = defineProps({
  name: String,
  description: String,
  profileLink: String,
  gitHubLink: String
});

/*const emit = defineEmits(
  ['childMessage']
);*/

</script>

<template>
  <Card class="card">
    <template #title><div v-if="profileLink"><h2><a :href="profileLink">{{ name }}</a></h2></div><div v-else><h2>{{ name }}</h2></div></template>
    <template #content>
      <div class="card-content-div">
        <div v-if="gitHubLink" class="github-div"><h3><a :href="gitHubLink">GitHub</a></h3></div>
        <div class="description-div">
          <p>{{description}}</p>
        </div>
      </div>

    </template>
  </Card>

</template>

<style scoped>

.card {
  margin: 5px;
  max-width: 600px;
  justify-content: flex-start;
  align-content: flex-start;
}

</style>
