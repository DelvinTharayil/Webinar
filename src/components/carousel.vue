<template>
  <v-carousel :show-arrows="true">
    <v-carousel-item
      v-for="(item,i) in items"
      :key="i"
      :src="item.src"
    ></v-carousel-item>
  </v-carousel>
</template>



<script>
  export default {
    data () {
      return {
        items: [
          {
            src: require("../assets/Screenshotwatch.png"),
          },
          {
            src:  require("../assets/Screenshotbreaking.png"),
          },
          {
            src:  require("../assets/Screenshot 2021-03-29 at 7.03.56 PM.png"),
          },
          {
            src:  require("../assets/Screenshotbreaking.png"),
          },
        ],
  }
 }
}
</script>