<template>
        <div class="whole">
            <h3>A Mádéfalvi Gyümölcs</h3>
            <div class="middle">
                <div class="line"></div>
                <v-img class="gajj" src="../assets/Gajjak 1.svg"></v-img>
                <div class="center">
                    <h3 class="grant">Garantátlja</h3>
                </div>
                <v-img class="gajj" src="../assets/Gajjak 2.svg"></v-img>
                <div class="line2"></div>
            </div>
            <h5>Helyi alapanyagból. Helyi erőforrásokkal. Helyi munkaerővel. Helyieknek.</h5>
        </div>
</template>

<script>
export default {
  name: "ProductGarantion",
};
</script>

<style scoped>
.whole{
    background-color: #F0F3F5;
    width: 100%;
    margin: 0 auto;
    padding: 37px 20px;
    display: flex;
    flex-direction: column;
    align-items: center;
    box-sizing: border-box;
}
h3{
    color: #08364D;
    font-family: fira-bold;
    font-size: 30px;
    line-height: 30px;
    letter-spacing: -1px;
    text-align: center;
}
.middle{
    width: 59%;
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    box-sizing: border-box;
    margin-top: 10px;
}
.line{
    width: 264px;
    height: 4px;
    border-radius: 10px;
    background-color: #08364D;
    margin-right: -10px;
}
.gajj{
    width: 150px !important;
    height: 70px;
}
.center{
    width: 320px;
    height: 70px;
    padding: 8px;
    border: 2px solid #08364D;
    border-radius: 10px;
    box-sizing: border-box;
}
.grant{
    font-size: 30px;
    line-height: 30px;
    border-radius: 5px;
    width: 100%;
    height: 100%;
    background-color: #E61437;
    display: flex;
    justify-content: center;
    align-items: center;
    color: #0F2733;
    font-family: fira-bold;
    box-sizing: border-box;
}
.line2{
    width: 264px;
    height: 4px;
    border-radius: 10px;
    background-color: #08364D;
    margin-left: -10px;
}
h5{
    margin-top: 21px;
    color: #08364D;
    font-family: fira-bold;
    font-size: 22px;
    line-height: 25px;
    letter-spacing: 0.8px;
    text-align: center;
}
</style>
