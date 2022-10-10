<template>
  <div class="container">
    <div class="row pt-5" style="background-color: #000">
      <hr style="border: 2px white solid; size: 1em; width: 100%" />
      <div class="col-md-6 justify-content-center">
        <div class="head">
          <p>
            InterconnectDATA <br />
            BreakPoint Podcast
          </p>
        </div>
      </div>
      <div class="col-md-6">
        <img :src="image" class="image-1" />
      </div>
      <hr
        class="mt-5"
        style="border: 2px white solid; size: 1em; width: 100%"
      />
      <div class="col-md-6 pt-5 justify-content-center">
        <div class="head">
          <p>
            InterconnectDATA <br />
            BreakPoint Podcast
          </p>
        </div>
      </div>
      <div class="col-md-6 pt-5">
        <img :src="image2" class="image-2" />
      </div>
      <hr
        class="mt-5"
        style="border: 2px white solid; size: 1em; width: 100%"
      />
      <div class="col-md-6 pt-5 justify-content-center">
        <div class="head">
          <p>
            InterconnectDATA <br />
            BreakPoint Podcast
          </p>
        </div>
      </div>
      <div class="col-md-6 pt-5">
        <img :src="image3" class="image-3" />
      </div>
      <hr
        class="mt-5"
        style="border: 2px white solid; size: 1em; width: 100%"
      />
      <div class="col-md-6 pt-5 justify-content-center">
        <div class="head">
          <p>
            InterconnectDATA <br />
            BreakPoint Podcast
          </p>
        </div>
      </div>
      <div class="col-md-6 pt-5">
        <img :src="image4" class="image-4" />
      </div>
      <hr
        class="mt-5"
        style="border: 2px white solid; size: 1em; width: 100%"
      />
      <div class="col-md-6 pt-5 justify-content-center">
        <div class="head">
          <p>
            InterconnectDATA <br />
            BreakPoint Podcast
          </p>
        </div>
      </div>
      <div class="col-md-6 pt-5">
        <img :src="image5" class="image-5" />
      </div>
      <hr
        class="mt-5"
        style="border: 2px white solid; size: 1em; width: 100%"
      />
      <div class="col-md-12 mt-5">
        <p class="headline">
          Lorem ipsum dolor sit amet, <br />
          consectetur adipiscing elit. <br />
          Morbi suscipit ante sem,
          <span style="font-style: italic">
            sed <br />
            interdum enim;</span
          >
        </p>
      </div>
      <div class="garis_verikal"></div>
    </div>
   </div>
  <Slider />
</template>

<script>
import image from "../assets/pic_1.png";
import image2 from "../assets/pic_2.png";
import image3 from "../assets/pic_3.png";
import image4 from "../assets/pic_4.png";
import image5 from "../assets/pic_5.png";
import Slider from "./Slider.vue";

export default {
  components: { Slider },
  data: function () {
    return {
      image: image,
      image2,
      image3,
      image4,
      image5,
    };
  },
};
</script>

<style lang="scss" scoped>
.image-1 {
  width: 30em;
}
.image-2 {
  width: 30em;
}
.image-3 {
  width: 30em;
}
.image-4 {
  width: 30em;
}
.image-5 {
  width: 30em;
}
.head {
  font-family: "Kanit";
  font-style: normal;
  font-weight: 300;
  font-size: 24px;
  line-height: 36px;
  text-align: justify;
  color: #ffffff;
}
.headline {
  font-family: "Kanit";
  font-style: normal;
  text-align: justify;
  font-weight: 700;
  font-size: 5em;
  margin-top: 2.5em;
  line-height: 97px;
  color: #ffffff;
}
.horizontal {
  border-left: 3px white solid;
  width: 331px;
  margin-bottom: 100px;
}
.garis_verikal {
  border-left: 3px white solid;
  height: 331px;
  margin-top: 15em;
}
</style>
