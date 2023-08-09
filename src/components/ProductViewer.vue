<template>
  <div>
    <div class="container">
      <div class="bal">
        <v-img
          class="leftbtn"
          src="../assets/navigate back.svg"
          @click="previousPicture"
        ></v-img>
      </div>
      <div class="pics">
        <v-img :src="currentPictureUrl" class="picture"></v-img>
      </div>
      <div class="bal">
        <v-img
          class="leftbtn"
          src="../assets/navigate forward.svg"
          @click="nextPicture"
        ></v-img>
      </div>
    </div>
    <div class="content">
      <div class="textbox">
        <v-img class="kep" src="../assets/Brand element 01.svg"> </v-img>
        <h1>Kerti Almalé</h1>
        <p>A MADÉFALVI ALMA ÁLMA.</p>
        <p class="long">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Pellentesque
          volutpat dolor lorem, id sodales lacus feugiat eget. Proin sed turpis
          est. Duis ac efficitur lorem, quis tempor turpis. Curabitur leo leo,
          lacinia in urna nec, vestibulum rhoncus arcu. Donec metus ipsum,
          rutrum non nulla a, luctus dictum arcu. Quisque laoreet elit nec dolor
          laoreet, quis blandit velit viverra. Sed accumsan nisi eget est
          elementum placerat. Nunc consectetur dignissim ipsum aliquet
          tristique. Donec quis enim non quam porttitor euismod quis nec sem.
          Sed molestie quam ac ex rhoncus sodales.<br /><br />
          Phasellus tempor arcu at eros rutrum viverra. Nam varius tempor lacus
          in cursus. Fusce aliquet volutpat nisi, scelerisque lobortis elit
          malesuada nec. Morbi eros tellus, tempor ut ipsum luctus, sagittis
          mollis nisl. Etiam mollis fermentum augue faucibus vestibulum. Nullam
          eget porta enim, vel placerat enim. Pellentesque euismod orci eu est
          consectetur fringilla. Phasellus placerat quam neque, at lacinia massa
          sollicitudin eu. Nullam vel lorem ullamcorper, molestie nunc nec,
          gravida libero. Nunc ac est in odio aliquet molestie euismod aliquam
          sem. Suspendisse viverra diam in nibh feugiat eleifend. Maecenas
          lacinia tortor eu ipsum sagittis, in faucibus purus faucibus.
          <br /><br />Curabitur ante est, ornare vitae sodales eu, porta eu
          turpis. Donec imperdiet, mauris ut feugiat elementum, mauris diam
          condimentum lorem, quis feugiat elit metus porttitor nisi. Vestibulum
          porttitor mi non turpis dignissim, vel porta nisi rhoncus.
          Pellentesque vehicula, ipsum at dignissim consectetur, justo neque
          euismod urna, id sollicitudin lacus purus quis dolor. Fusce egestas
          convallis libero, quis placerat lorem consequat vitae. Aliquam eros
          orci, rhoncus sit amet massa sed, rhoncus facilisis nunc. Nunc magna
          libero, dapibus fermentum enim sed, faucibus elementum justo.
          Phasellus et interdum diam, vel viverra neque. Ut volutpat enim eu
          sapien ultrices, a ornare elit condimentum. In posuere felis et
          tincidunt consequat. Ut at felis hendrerit, tristique orci nec, rutrum
          mi. Ut lectus ante, ornare in posuere a, sodales vitae leo. Vestibulum
          quis arcu consectetur, dictum orci nec, ornare libero. Ut a urna id
          eros mollis mollis. Nulla tortor arcu, rhoncus vitae consequat in,
          lobortis vitae enim.
        </p>
        <v-img class="kep" src="../assets/Brand element 02.svg"> </v-img>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "ProductViewer",
  data() {
    return {
      pictureIndex: 0,
      pictures: [
        require("@/assets/prod.jpg"),
        require("@/assets/prod1.jpg"),
        require("@/assets/prod2.jpg"),
      ],
    };
  },
  computed: {
    currentPictureUrl() {
      return this.pictures[this.pictureIndex];
    },
  },
  methods: {
    nextPicture() {
      this.pictureIndex = (this.pictureIndex + 1) % this.pictures.length;
    },
    previousPicture() {
      this.pictureIndex =
        (this.pictureIndex - 1 + this.pictures.length) % this.pictures.length;
    },
  },
};
</script>

<style scoped>
.container {
  width: 100%;
  padding: 61px 16px 191px;
  background-color: #7a8f99;
  position: relative;
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  gap: 0px 32px;
  box-sizing: border-box;
}
.bal {
  background-color: white;
  border-radius: 3px;
  padding: 8px 8px 4px;
  box-shadow: 0px 1px 2px #677d8433;
  cursor: pointer;
}
.leftbtn {
  width: 24px;
  height: 24px;
}
.pics {
  flex: 1 1 0%;
  max-width: 936px;
  border-radius: 12px;
}
.picture {
  width: 936px;
  height: 598px;
  border-radius: 12px;
}
.content {
  width: 100%;
  padding-left: 16px;
  padding-right: 16px;
  background-color: white;
  position: relative;
  box-sizing: border-box;
}
.textbox {
  width: 60%;
  background-color: white;
  border-radius: 12px;
  box-shadow: 0px 50px 80px #0d988c1a;
  position: relative;
  top: -130px;
  box-sizing: border-box;
  margin: 0 auto;
  padding: 83px 96px 73px;
  display: flex;
  flex-direction: column;
  align-items: center;
}
.kep {
  width: 50px;
  height: 40px;
  margin: 0 auto;
  margin-top: 83px;
}
h1 {
  font-size: 80px;
  font-family: fira-bold;
  color: #08364d;
  letter-spacing: 0.08;
  margin-top: 55px;
}
p {
  color: #e61437;
  font-size: 24px;
  letter-spacing: 0.0384;
  font-family: fira-bold;
}
.long {
  margin-top: 113px;
  text-align: center;
  font-size: 24px;
  line-height: 32px;
  font-weight: 500;
  letter-spacing: 0.784;
  font-family: fira-regular;
  color: #0f2733;
}
</style>
