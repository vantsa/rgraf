<template>
  <v-app>
    <v-main>
      <router-view/>
    </v-main>
  </v-app>
</template>

<script>

export default {
  name: 'App',

  data: () => ({
    //
  }),
};
</script>
<style scoped>
@font-face {
  font-family: "fira-bold";
  src: local("FiraSans-Bold"),
   url(assets/fonts/FiraSans-Bold.ttf) format("truetype");
}
@font-face {
  font-family: "fira-regular";
  src: local("FiraSans-Regular"),
   url(assets/fonts/FiraSans-Regular.ttf) format("truetype");
}
@font-face {
  font-family: "roboto-regular";
  src: local("Roboto-Regular"),
   url(assets/fonts/Roboto-Regular.ttf) format("truetype");
}
@font-face {
  font-family: "roboto-medium";
  src: local("Roboto-Medium"),
   url(assets/fonts/Roboto-Medium.ttf) format("truetype");
}
</style>
