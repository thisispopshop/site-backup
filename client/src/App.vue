<!--The main page of your site-->

<template>
  <div id="app">

    <!--tab title thing-->
    <vue-headful
        title="Popshop"
    />

      <RouterView/>

      <footer class="footer my-footer">
          
            <div class="content has-text-centered">
                <p>
                  <b>© Popshop 2019</b> 
                  <!--social media not ready
                    <br>
                  <a class="tab-space" href="https://www.facebook.com/Popshop-384434792395944/" target="_blank">
                    <font-awesome-icon :icon="{ prefix: 'fab', iconName: 'facebook' }"/>
                  </a>
                  <span class="tab-space"><font-awesome-icon :icon="{ prefix: 'fab', iconName: 'twitter' }"/></span>
                  <span class="tab-space"><font-awesome-icon :icon="{ prefix: 'fab', iconName: 'instagram' }"/></span>
                  -->
                </p>
            </div>
      </footer>
  </div>
</template>

<script lang="ts">
/* eslint-disable */

//import axios from "axios";
import Vue from "vue";
import { Component }  from "vue-property-decorator";

@Component
export default class App extends Vue {}
</script>


<style lang="scss">

//custom bulma variables
//we can create the theme here!

$input-focus-border-color:transparent;
$input-focus-box-shadow-color:transparent;
$input-shadow: none;
$input-border-color: transparent;

$navbar-dropdown-boxed-radius: 0px;
$navbar-height: 7rem;
$navbar-item-img-max-height: 7rem;

$dropdown-item-active-background-color: none;

$family-primary: 'Brandon Grotesque', sans-serif;

@import "~bulma/css/bulma.css";
@import "bulma/sass/utilities/_all.sass";
@import "bulma/sass/grid/columns.sass";
@import "bulma/bulma.sass";

@font-face {
  font-family: "Brandon Grotesque";
  src: url('./assets/fonts/Brandon_light.otf');
      font-weight: normal;
      font-style: normal;
}

#app {
  font-family: "Brandon Grotesque", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}

//add slight tabbing
.tab-space {
  padding-left:1em 
}

//change link color to none
a:link {
  color:none;
}

body {
  background: #F8F8F8
}

.my-footer {
  background: #F5F5F5;
}

</style>
