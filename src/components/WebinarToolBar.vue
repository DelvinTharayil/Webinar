<template>
  <v-card class="overflow-hidden">
    <v-app-bar
      fixed
      color="white"
      style="height: 70px"
      elevate-on-scroll
      scroll-target="#scrolling-techniques-7"
    >
      <v-toolbar-title class="mytitle"
        >scool<span style="color: rgba(242, 36, 49, 1)"
          >.</span
        ></v-toolbar-title
      >

      <v-spacer></v-spacer>
    </v-app-bar>
    <v-sheet
      id="scrolling-techniques-7"
      class="overflow-y-auto"
      style="max-height: 100vh"
    >
      <v-container fluid class="container">
      <div>
      <WebinarContent/>
     </div>
      </v-container>
    </v-sheet>
  </v-card>
</template>

<style>
@import url("https://fonts.googleapis.com/css2?family=Montserrat:wght@100;700&display=swap");
 .mytitle {
  font-family: "Montserrat", sans-serif;
  font-weight: bold;
  font-size: 48px !important;
  padding: 2.5% ;
}
.container{
  height: 100vh;
  padding: 60px 2.5%  ;
}



</style>

<script>
import WebinarContent from '../components/WebinarContent';

export default {

  components: {
    WebinarContent,
  },
};
</script>