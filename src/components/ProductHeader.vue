<template>
  <div class="container">
    <div class="box">
      <h5 @click="goToMainPage">Rólunk</h5>
    </div>
    <div class="box2"></div>
    <div class="box3">
      <h5>Termékeink</h5>
    </div>
    <div class="huro">
      <div class="content">
        <div class="button">
          <h5 :class="{ active: activeButton === 'Hu' }" @click="activeButton = 'Hu'">Hu</h5>
          <h5 :class="{ active: activeButton === 'Ro' }" @click="activeButton = 'Ro'">Ro</h5>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "PageHeader",
  data() {
    return {
      activeButton: "Hu"
    }
  },
  methods: {
    goToMainPage() {
        this.$router.push("/")
    }
  }
};
</script>

<style scoped>
.container {
  width: 100%;
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  gap: 0 70px;
  padding: 30px 20px;
  box-sizing: border-box;
  position: sticky;
  top: 0;
  z-index: 9999;
  background-color: white;
}
.container .box {
  flex: 1 1 0%;
  display: flex;
  flex-direction: row-reverse;
}
h5 {
  font-size: 20px;
  letter-spacing: -0.3px;
  font-family: fira-bold;
  color: #08364d;
  cursor: pointer;
}
.container .box2 {
  width: 150px;
  height: 70px;
  background-image: url("../assets/Logo small.svg");
  background-size: contain;
  background-repeat: no-repeat;
  background-position: center center;
  transition: all 0.3s ease 0s;
  cursor: pointer;
}
.container .box3 {
  flex: 1 1 0%;
  display: flex;
  flex-direction: row;
}
.huro {
  position: absolute;
  right: 370px;
}
.content {
  width: 104px;
  height: 56px;
  padding: 5px;
  background-color: white;
  box-shadow: 0px 3px 6px #00000029;
  border-radius: 4%;
  cursor: pointer;
}
.button {
  display: flex;
  flex-direction: row;
  -webkit-box-pack: justify;
  justify-content: space-between;
  background-color: #F0F3F5;
  border-radius: 3px;
}
.button h5{
    width: 46px;
    height: 46px;
    display: flex;
    font-size: 16px;
    align-items: center;
    font-family: fira-bold;
    border-radius: 3px;
    justify-content: center;
}
.button h5.active {
  background-color: #E61437;
  color: white;
}

.button h5:not(.active) {
  background-color: #F0F3F5;
  color: #08364D;
}
</style>
