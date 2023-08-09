<template>
        <div class="img-withtext">
            <div class="imgbox">
                <v-img class="img" src="../assets/alma1.jpeg"> </v-img>
            </div>
            <div class="textbox">
                <div class="content">
                    <h2>Ma délelőtt a nap éltető sugarai ébresztették az érő gyümölcsöt.</h2>
                    <h4>UT ENIM AD MINIMA VENIAM</h4>
                    <button class="button1">TOVÁBB</button>
                </div>
            </div>
        </div>
</template>

<script>
export default {
  name: "FirstContent",
};
</script>

<style scoped>
.img-withtext {
    width: 100%;
    display: flex;
    flex-direction: row;
    align-items: stretch;
    gap: 48px 0px;
    box-sizing: border-box;
    margin-bottom: 100px;
}
.imgbox{
    width: 48%;
    display: flex;
    -webkit-box-pack: center;
    justify-content: center;
    -webkit-box-align: center;
    align-items: center;
}
.textbox{
    background-color: #08364d;
    width: 100%;
    display: flex;
    justify-content: center;
    
}
.textbox .content{
    flex: 1 1 0%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    padding: 48px 20px;
    box-sizing: border-box;
}
h2{
    color: white;
    margin: 0px 0px 20px 50px;
    font-family: fira-bold;
    font-size: 50px;
    line-height: 60px;
    letter-spacing: -1px;
    max-width: 55%;
    overflow-wrap: break-word;
    word-break: break-word;
}
h4{
    margin: 0px 0px 80px;
    font-family: fira-bold;
    font-size: 24px;
    line-height: 28px;
    color: #E61437;
    margin-left: 50px;
    margin-bottom: 80px;
}
.button1{
    display: inline-flex;
    align-items: center;
    justify-content: center;
    position: relative;
    box-sizing: border-box;
    border: 0px;
    margin: 0px;
    cursor: pointer;
    vertical-align: middle;
    appearance: none;
    text-decoration: none;
    font-weight: 500;
    line-height: 1.75;
    padding: 8px 22px;
    color: white;
    background-color: #E61437;
    width: 200px;
    height: 48px;
    font-family: Roboto;
    font-size: 20px;
    border-radius: 6px;
    margin-left: 50px;
}
.img{
    height: 810px;
}
</style>
