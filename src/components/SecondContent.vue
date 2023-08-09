<template>
  <div class="content">
    <v-img class="kep" src="../assets/Brand element 01.svg"> </v-img>
    <h5>Madéfalva neve a Szeresd az Istent!</h5>
    <p>
      Madéfalva neve a Szeresd az Istent! parancsolat latin nevéből ered. Annak
      a felismeréséből származik, hogy az Isten szeretete ösztönös, belülről
      jövő késztetés, hogy az emberi szellemnek úgy része ez a parancsolat,
      ahogyan a pataknak is van elve, amit követnie kell.
    </p>
    <div class="circle"></div>
  </div>
</template>

<script>
export default {
  name: "SecondContent",
};
</script>

<style scoped>
.content {
  margin: 0 auto;
  width: 83%;
  margin-top: 150px;
}
.kep {
  width: 3%;
  margin: 0 auto;
}
h5 {
  margin: 25px 0px 50px;
  font-weight: 400;
  color: #e61437;
  font-family: fira-bold;
  font-size: 50px;
  line-height: 60px;
  letter-spacing: -1px;
  text-align: center;
}
p {
  font-family: fira-regular;
  font-size: 28px;
  line-height: 32px;
  font-weight: 500;
  letter-spacing: 0.784;
  text-align: center;
  width: 63%;
  margin: 0 auto;
  color: #0f2733;
}
.circle {
  background-color: #e61437;
  border-radius: 50%;
  width: 12px;
  height: 12px;
  margin: 0 auto;
  margin-top: 50px;
}
</style>