<template>
  <!-- <div class="page">
    <nav id="colorlib-main-nav" role="navigation">
      <a href="#" class="js-colorlib-nav-toggle colorlib-nav-toggle active"
        ><i></i
      ></a>
      <div class="js-fullheight colorlib-table">
        <div class="img" style="background-image: url(images/bg_3.jpg)"></div>
        <div class="colorlib-table-cell js-fullheight">
          <div class="row no-gutters">
            <div class="col-md-12 text-center">
              <h1 class="mb-4">
                <a href="index.html" class="logo">Company Logo</a>
              </h1>
              <ul>
                <li class="active">
                  <a href="index.html"><span>Home</span></a>
                </li>
                <li>
                  <a href="about.html"><span>About</span></a>
                </li>
                <li>
                  <a href="blog.html"><span>Blog</span></a>
                </li>
                <li>
                  <a href="contact.html"><span>Contact</span></a>
                </li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </nav>

    <div id="colorlib-page">
      <header>
        <div class="container">
          <div class="colorlib-navbar-brand">
            <a class="colorlib-logo" href="index.html">Company Logo</a>
          </div>
          <a href="#" class="js-colorlib-nav-toggle colorlib-nav-toggle"
            ><i></i
          ></a>
        </div>
      </header>
    </div>
  </div> -->
  <Headbody />
</template>

<script>
import Headbody from "./HeadBody.vue";

export default {
  name: "App",
  components: {
    Headbody,
  },
};
</script>

<style lang="scss" scoped>
$font-primary: "Poppins", Arial, sans-serif;
$primary: #fec771;

body {
  font-family: $font-primary;
  font-size: 16px;
  line-height: 1.8;
  font-weight: normal;
  background: #fafafa;
  color: lighten(#000, 50%);
  &.menu-show {
    overflow: hidden;
    position: fixed;
    height: 100%;
    width: 100%;
  }
}
a {
  transition: 0.3s all ease;
  color: $primary;
  &:hover,
  &:focus {
    text-decoration: none !important;
    outline: none !important;
    box-shadow: none;
  }
}
h1,
h2,
h3,
h4,
h5,
.h1,
.h2,
.h3,
.h4,
.h5 {
  line-height: 1.5;
  font-weight: 400;
  font-family: $font-primary;
  color: #000;
}

.bg-primary {
  background: $primary !important;
}

.ftco-section {
  padding: 7em 0;
}

.ftco-no-pt {
  padding-top: 0;
}
.ftco-no-pb {
  padding-bottom: 0;
}
//HEADING SECTION
.heading-section {
  font-size: 28px;
  color: #000;
}

//COVER BG
.img {
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center center;
}

#colorlib-main-nav {
  position: absolute;
  top: 0;
  bottom: 0;
  right: 0;
  padding: 0;
  width: 100%;
  height: 100%;
  background: rgba(#000, 0.99);
  z-index: 1002;
  text-align: center;
  visibility: hidden;
  opacity: 0;
  -webkit-transition: all 0.8s cubic-bezier(0.175, 0.885, 0.32, 1.275);
  -moz-transition: all 0.8s cubic-bezier(0.175, 0.885, 0.32, 1.275);
  -ms-transition: all 0.8s cubic-bezier(0.175, 0.885, 0.32, 1.275);
  -o-transition: all 0.8s cubic-bezier(0.175, 0.885, 0.32, 1.275);
  transition: all 0.8s cubic-bezier(0.175, 0.885, 0.32, 1.275);
  -webkit-transform: scale(0.1);
  -moz-transform: scale(0);
  -ms-transform: scale(0);
  -o-transform: scale(0);
  transform: scale(0);
  overflow-y: scroll;
  .colorlib-table {
    display: table;
    width: 100%;
    height: 100%;
    .img {
      position: absolute;
      top: 0;
      left: 0;
      bottom: 0;
      height: 100%;
      width: 100%;
      opacity: 1;
      &:after {
        position: absolute;
        top: 0;
        left: 0;
        bottom: 0;
        right: 0;
        content: "";
        background: rgba(#000, 0.3);
      }
    }
    .colorlib-table-cell {
      display: table-cell;
      vertical-align: middle;
    }
  }
  .colorlib-nav-toggle {
    position: absolute;
    top: 40px;
    right: 40px;
    padding: 20px;
    height: 44px;
    width: 44px;
    line-height: 0;
    padding: 0 !important;
    visibility: hidden;
    opacity: 0;
    transition: 3s;
    i {
      top: 18px !important;
      left: 0 !important;
      margin: 0 !important;
      padding: 0 !important;
      line-height: 0;
      text-indent: 0;
    }
    &.show {
      visibility: visible;
      opacity: 1;
    }
    &:hover {
      // background: rgba(0,0,0,1);
      i {
        &::before,
        &::after {
          content: "";
          width: 40px;
          height: 2px;
          background: #000;
          position: absolute;
          left: 0;
        }
      }
    }
  }
  .menu-show & {
    visibility: visible;
    opacity: 1;
    -webkit-transform: scale(1);
    -moz-transform: scale(1);
    -ms-transform: scale(1);
    -o-transform: scale(1);
    transform: scale(1);
  }
  .logo {
    font-size: 40px;
    color: #000;
    text-transform: uppercase;
    letter-spacing: 2px;
    font-weight: 700;
    position: relative;
    display: inline-block;
    margin-bottom: 0;
    line-height: 1.5;
    font-family: $font-primary;
    span {
      font-size: 14px;
      display: block;
      font-weight: 300;
      color: rgba(255, 255, 255, 0.8);
      letter-spacing: 8px;
    }
  }
  ul {
    padding: 0;
    margin: 0;
    display: block;
    media-brea:oit-down(sm) {
      padding: 20px 0 0 0;
    }
    li {
      padding: 0;
      margin: 0;
      list-style: none;
      font-weight: 600;
      font-size: 14px;
      letter-spacing: 5px;
      text-transform: uppercase;
      a {
        display: block;
        color: rgba(255, 255, 255, 1);
        padding: 5px 0;
        span {
          color: rgba(255, 255, 255, 1);
          position: relative;
          padding: 0 10px;
          small {
            position: absolute;
            bottom: 7px;
            left: -30px;
            font-size: 16px;
            color: rgba(255, 255, 255, 0.3);
            border-bottom: 1px solid rgba(255, 255, 255, 0.3);
          }
        }
        &:hover,
        &:active,
        &:focus {
          outline: none;
          text-decoration: none;
          span {
            &:before {
              visibility: visible;
              -webkit-transform: scaleX(1);
              -moz-transform: scaleX(1);
              -ms-transform: scaleX(1);
              -o-transform: scaleX(1);
              transform: scaleX(1);
            }
          }
        }
      }
      &.active {
        a {
          span {
            color: #f8b500;
            &:before {
              background: $primary;
              visibility: visible;
              -webkit-transform: scaleX(1);
              -moz-transform: scaleX(1);
              -ms-transform: scaleX(1);
              -o-transform: scaleX(1);
              transform: scaleX(1);
            }
          }
        }
      }
    }
  }
}

///////////////
header {
  padding: 2em 0;
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  z-index: 9;
  margin: 0 auto;
  media-brea:oit-down(sm) {
    padding: 1em 0;
    position: absolute;
  }
  .colorlib-navbar-brand {
    float: left;
    .colorlib-logo {
      font-size: 12px;
      color: #000;
      letter-spacing: 5px;
      font-weight: 600;
      position: relative;
      display: inline-block;
      margin-bottom: 0;
      line-height: 1.5;
      font-family: $font-primary;
      text-transform: uppercase;
      span {
        font-size: 11px;
        display: block;
        font-weight: 300;
        color: rgba(255, 255, 255, 0.8);
        letter-spacing: 7px;
      }
      i {
        color: $primary;
        position: absolute;
        top: -18px;
        bottom: 0;
        left: 7px;
        font-size: 48px;
      }
      &:hover {
        text-decoration: none !important;
      }
      &:active,
      &:focus {
        outline: none;
        text-decoration: none;
      }
    }
  }
}

///////////////
.colorlib-nav-toggle {
  cursor: pointer;
  text-decoration: none;
  &.active i {
    &::before,
    &::after {
      background: #000;
    }
  }
  &.dark {
    &.active i {
      &::before,
      &::after {
        background: #000;
      }
    }
  }
  &:hover,
  &:focus,
  &:active {
    outline: none;
    border-bottom: none !important;
  }
  i {
    position: relative;
    display: inline-block;
    width: 20px;
    height: 2px;
    color: #000;
    font: bold 14px/0.4 Helvetica;
    text-transform: uppercase;
    text-indent: -55px;
    background: #000;
    transition: all 0.2s ease-out;
    .menu-show & {
      background: #000;
      color: #000;
    }
    &::before,
    &::after {
      content: "";
      width: 30px;
      height: 2px;
      background: #000;
      position: absolute;
      left: 0;
      .menu-show & {
        background: #000;
      }
      transition: 2s;
    }
  }
  &.dark {
    i {
      position: relative;
      color: #000;
      background: #000;
      transition: all 0.2s ease-out;
      &::before,
      &::after {
        background: #000;
        transition: 2s;
      }
    }
  }
}

.colorlib-nav-toggle i::before {
  top: -7px;
}
.colorlib-nav-toggle i::after {
  bottom: -7px;
}
.colorlib-nav-toggle:hover i::before {
  top: -10px;
}
.colorlib-nav-toggle:hover i::after {
  bottom: -10px;
}
.colorlib-nav-toggle.active i {
  background: transparent;
}
.colorlib-nav-toggle.active i::before {
  top: 0;
  -webkit-transform: rotateZ(45deg);
  -moz-transform: rotateZ(45deg);
  -ms-transform: rotateZ(45deg);
  -o-transform: rotateZ(45deg);
  transform: rotateZ(45deg);
}
.colorlib-nav-toggle.active i::after {
  bottom: 0;
  -webkit-transform: rotateZ(-45deg);
  -moz-transform: rotateZ(-45deg);
  -ms-transform: rotateZ(-45deg);
  -o-transform: rotateZ(-45deg);
  transform: rotateZ(-45deg);
}
.colorlib-nav-toggle {
  float: right;
  z-index: 1003;
  position: relative;
  top: 0;
  right: 0;
  display: block;
  margin: 0 auto;
  cursor: pointer;
  margin-top: 0;
  media-brea:oit-down(sm) {
    right: 10px;
  }
}

.hero-wrap {
  background: #202020;
  .slider-text {
    .desc {
      h1 {
        font-size: 6vw;
        font-weight: 700;
        color: #000;
        text-transform: uppercase;
      }
      h3 {
        color: rgba(255, 255, 255, 0.8);
        font-size: 18px;
      }
    }
  }
}
</style>
