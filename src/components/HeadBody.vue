<template>
  <div class="container" style="background-color: #000">
    <div class="row">
      <div class="col-6" >
        <h1
          class="text-left text-white heading"
          style="text-align: left;  margin-top: 300px"
        >
          Lorem ipsum dolor sit <br />
          amet,
          <span class="subhead" style="font-style: italic">
            consectetur <br />
            adipiscing elit.</span
          >
        </h1>
      </div>
      <div class="col-6" style="background-color: #000">
        <h5
          style="
            margin-top: 300px;
            text-align: justify;
            color: #fff;
          "
          class="subheading"
        >
          Quisque quis turpis aliquam, aliquet nibh id, condimentum nunc. Morbi
          massa lacus, pulvinar ac posuere quis, pharetra id tortor. Sed
          facilisis lectus quis dignissim luctus. Curabitur rhoncus nec ipsum eu
          viverra. Donec quam nibh, rutrum id bibendum a, accumsan et elit.
        </h5>
        <h5
          class="pt-5 sub-head"
          style="text-align: justify; color: #fff"
        >
          Nunc dui mi, varius non risus eget, imperdiet cursus urna. Lorem ipsum
          dolor sit amet, consectetur adipiscing elit. Phasellus tincidunt
          lectus ac blandit sollicitudin. Ut vel dolor scelerisque, posuere
          sapien sed, imperdiet ligula. Fusce mattis vestibulum nibh vitae
          faucibus. Ut feugiat ex in nisi elementum cursus. Duis vehicula
          consequat nisi eget facilisis. Aenean dui turpis, elementum eleifend
          libero ultrices, rhoncus dictum dolor.
        </h5>
      </div>
      <div class="col-6" style="background-color: #000">
        <div class="garis_verikal"></div>
        <h1
          style="
            text-align: justify;
            color: #fff;
            font-size: 64px;
          "
          class="recent"
        >
          Recent
          <span style="font-style: italic"
            ><br />
            Work
          </span>
        </h1>
      </div>
      <div class="col-6" style="background-color: #000"></div>
    </div>
  </div>

  <SectionWork />
</template>

<script>
import SectionWork from "./SectionWork.vue";

export default {
  name: "App",
  components: {
    SectionWork,
  },
};
</script>

<style lang="scss" scoped>
.heading {
  font-family: "kanit";
}
.span {
  font-family: "Playfair Display";
}

.garis_verikal {
  border-left: 3px white solid;
  height: 331px;
  margin-left: 5  em;
  margin-bottom: 100px;
}

@media (max-width: 600px) {
  .heading {
    text-align: left !important;
    font-size: 16px !important;
    margin-left: 3em !important;
    margin-top: 5em !important;
  }
  .subheading {
    font-size: 1em;
    margin-right: 1em !important;
    text-align: justify;
    margin-top: 5em !important;
  }
  .sub-head {
    font-size: 1em;
    margin-right: 1em !important;
    text-align: justify;
    margin-top: 0.1em !important;
  }
  .recent {
    font-size: 2em !important;
    margin-left: 2em !important;
    margin-top: -10em !important;
    margin-bottom: 2em !important;
  }
  .garis_vertikal {
    margin-left: 10px !important;
    display: none;
  }
}
</style>
