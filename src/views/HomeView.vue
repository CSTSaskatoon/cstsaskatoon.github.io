<script setup lang="ts">

import ProfileCard from '@/components/ProfileCard.vue'
</script>

<template>
<div>
  <h1>Welcome to the CST Saskatoon Group Portfolio page!</h1>
  <div class="profile-cards">
    <ProfileCard :name="'Denali'" :profile-link="'https://denalitherrien.github.io'" :git-hub-link="'https://github.com/denalitherrien'" :description="'Gamer'" />
  </div>
</div>
</template>

<style scoped>

div {
  display: flex;
  justify-content: center;
  align-content: center;
  flex-wrap: wrap;
  flex-direction: column;
  flex-grow: 1;
  width: 100%;
}



</style>
