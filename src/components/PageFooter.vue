<template>
  <div class="container">
    <v-img class="logo" src="../assets/Logo small.svg"></v-img>
    <p>Cím: <span class="b">Siculeni 106, 537295, HR.</span></p>
    <p>Telefon: <span class="b">0266 379107</span></p>
    <p>Fax: <span class="b"> 0266 316951</span></p>
    <p>Email: <span class="b">madefalva@yahoo.com</span></p>
    <div class="social">
        <v-img class="icon" src="../assets/FB.svg"></v-img>
        <v-img class="icon" src="../assets/Tw.svg"></v-img>
        <v-img class="icon" src="../assets/Mail.svg"></v-img>
    </div>
  </div>
</template>

<script>
export default {
  name: "PageFooter",
};
</script>

<style scoped>
.container {
  width: 100%;
  background-color: #08364d;
  padding: 86px 20px 63px;
  display: flex;
  flex-direction: column;
  align-items: center;
  box-sizing: border-box;
}
.logo {
  width: 160px;
  height: 84px;
  margin: 0 auto;
  margin-bottom: 32px;
}
p {
  color: white;
  font-size: 16px;
  line-height: 0.2;
  font-family: roboto-regular;
  letter-spacing: 0.5px;
}
.b {
  font-family: roboto-medium;
}
.social {
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  gap: 24px;
  margin-top: 40px;
}
.icon{
    width: 30px;
    height: 30px;
}
</style>
