<template>
    <div>
      <img :src="avatar" :alt="alt"  />
      <!-- usando v-bind de forma resumida = : scr/herf ....-->
    </div>
  </template>
  
  <script>
  export default {
    name: 'Picture',
    data() {
      return {
        avatar: "/img/avatar.jpg",
        alt: "profile_photo",
      };
    },
  };
  </script>