<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* text-align: center; */
  color: #2c3e50;

}

@font-face{
    font-family: "GBold";
    src: url("assets/TTF/Bold.ttf");
    /* font-weight: bold; */
}

@font-face {
    font-family: "GMedium";
    src: url("assets/TTF/Medium.ttf");
    /* font-weight: normal; */
}

@font-face {
    font-family: "GLight";
    src: url("assets/TTF/Light.ttf");
    /* font-weight: light; */
}
  

g-light {
    font-family: "GLight";
    font-style: normal;
    font-weight: normal;
}

g-medium {
    font-family: "GMedium";
    font-style: normal;
    font-weight: normal;
}

g-bold {
    font-family: "GBold";
    font-style: normal;
    font-weight: normal;
}

</style>
