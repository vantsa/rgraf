<template>
        <div class="content">
            <v-img class="kep" src="../assets/Brand element 02.svg"> </v-img>
            <h5>Amadéfalva</h5>
            <p>Eredeti neve Amadéfalva volt. Első birtokosáról kapta a nevét. A falut már 1333-ban említik Csíkrákos fiókegyházaként, de önálló községként csak 1567-ben szerepel még Amadéfalva néven. <br><br>1764. január 7-én az osztrák császári katonaság itt mészárolt le több száz székelyt, akik tiltakoztak a határőrezred felállítása ellen, és az adóztatás ellen. Ezt a gyalázatos eseményt „siculicidiumnak” vagy „madéfalvi veszedelemnek” nevezik. Ezután indult meg a székelyek tömeges kivándorlása. 1910-ben 1908, túlnyomórészt magyar lakosa volt. <br>A trianoni békeszerződésig Csík vármegye Felcsíki járásához tartozott. 1992-ben 2812 lakosából 2644 magyar és 167 román volt.</p>
            <div class="circle"></div>
        </div>
</template>

<script>
export default {
  name: "FourthContent",
};
</script>

<style scoped>
.content{
    margin: 0 auto;
    width: 83%;
    margin-top : 150px;
}
.kep{
    width: 3%;
    margin: 0 auto;
}
h5{
    margin: 25px 0px 50px;
    color: #E61437;
    font-family: fira-bold;
    font-size: 50px;
    line-height: 60px;
    letter-spacing: -1px;
    text-align: center;
}
p{
    font-family: fira-regular;
    font-size: 28px;
    line-height: 40px;
    letter-spacing: 0.784;
    font-weight: 500;
    text-align: left;
    width: 58%;
    margin: 0 auto;
    color: #0f2733;
}
.circle{
    background-color: #E61437;
    border-radius: 50%;
    width: 12px;
    height: 12px;
    margin: 0 auto;
    margin-top: 50px;
    margin-bottom: 162px;
}
</style>
