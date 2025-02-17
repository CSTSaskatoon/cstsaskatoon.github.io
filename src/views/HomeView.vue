<script setup lang="ts">

import ProfileCard from '@/components/ProfileCard.vue'

const denaliDescription: string = "Seeking a career that allows me to apply my expertise in" +
  " communication networks, computer engineering, programming, cloud architectures," +
  " and application development to grow with an innovative company throughout my career." +
  " My experience in software development has equipped me with the ability to design, implement," +
  " and optimize network-driven applications while ensuring reliability and scalability." +
  " I am particularly interested in working with Cloud infrastructure and virtual network functions." +
  " I remain excited about the opportunity to apply my skills to support and enhance" +
  " advanced technical infrastructure."

const exampleDescription: string = "Lorem ipsum dolor sit amet, consectetur adipiscing elit." +
  " Vivamus pharetra, quam quis condimentum luctus, felis urna scelerisque felis, a porttitor ante" +
  " lorem sit amet mi. Interdum et malesuada fames ac ante ipsum primis in faucibus." +
  " Ut volutpat neque molestie purus tempus, vitae cursus turpis rhoncus." +
  " Morbi eu justo id enim tincidunt ornare non at est. Donec nec ultrices lacus, id sollicitudin dui." +
  " Maecenas volutpat vehicula tortor, a aliquet quam iaculis venenatis." +
  " Sed nisl orci, fringilla quis dapibus vel, suscipit id mauris." +
  " Morbi viverra bibendum sapien quis pulvinar. Proin lacinia facilisis imperdiet." +
  " Proin dignissim lacus eget sollicitudin scelerisque." +
  " Cras vitae lacus convallis arcu consectetur ultrices non sed elit. "
</script>

<template>
<div>
  <h1>Welcome to the CST Saskatoon Group Portfolio page!</h1>
  <div class="profile-cards">
    <ProfileCard
      :name="'Denali'"
      :profile-link="'https://denalitherrien.github.io'"
      :git-hub-link="'https://github.com/denalitherrien'"
      :description="denaliDescription" />
    <ProfileCard
      :name="'Example'"
      :profile-link="'https://pages.github.com'"
      :git-hub-link="'https://github.com'"
      :description="exampleDescription" />
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
