<template>
  <div class="content">
    <v-img class="kep" src="../assets/Brand element 01.svg"> </v-img>
    <h5>Jézus Szíve tiszteletére</h5>
    <p>
      A település fontosabb részei Patakelve, Alszeg, Vargaszeg, Állomás
      környéke, és a Főút mellett. A falu plébánosa Bartalus Jakab Zoltán. A
      „Zöld Péter” Általános Iskola igazgatója Máté Sándor. <br><br>Az 1764. évi
      mészárlás helyén 1905. október 8-án avatták fel az emlékművet Köllő Miklós
      alkotását, a helyén egykor állt sírkereszt a csíkszentmihályi templom
      kertjében áll. Római katolikus temploma 1913-14-ben épült Jézus Szíve
      tiszteletére.
    </p>
    <div class="circle"></div>
  </div>
</template>

<script>
export default {
  name: "SixthContent",
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
  line-height: 40px;
  letter-spacing: 0.784;
  font-weight: 500;
  text-align: center;
  width: 70%;
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