<template>
  <v-container fluid grid-list-lg>
    <v-layout row wrap>
      <v-flex d-flex align-end xs12 sm6 md8>
        <v-layout row wrap>
          <v-card style="border-radius: 16px !important">
            <v-img
              style="max-width: 1000px"
              src="../assets/Screenshot 2021-03-29 at 7.03.56 PM.png"
            ></v-img>
            <v-card-title primary class="title">Iphone videography for product</v-card-title>
            <v-card-text class="Coursetext">{{
              lorem.slice(0, 70)
            }}</v-card-text>
          </v-card>
          <v-flex>
            <v-card style="border-radius: 16px !important">
              <v-card-title primary class="title">Brief Description</v-card-title>
              <v-card-text class="Coursetext">{{
                lorem.slice(0, 70)
              }}</v-card-text>
            </v-card>
          </v-flex>
        </v-layout>
      </v-flex>
      <v-flex d-flex xs12 sm6 md4>
        <v-card>
                  <v-img
                  class="primaryimg"
                    style="border-radius: 0px !important"
                    width="300"
                    height="300"
                    aspect-ratio="1.7"
                    src="../assets/Screenshotmen.png"
                  >
                  </v-img>
                  <v-card-title
                    primary
                    class="title justify-center"
                    style="color: #F3164D "
                    >Deepak Shapeti</v-card-title
                  >
                  <v-card-title class="justify-center"
                    >Obsessive Serial Entrepreneur</v-card-title
                  >
                  <v-card-text class="justify-center"
                    >{{ lorem}}
                  </v-card-text>
                  <v-chip-group
                    style="margin: 20px"
                    v-model="selection"
                    active-class="red accent-3 white--text"
                    column
                  >
                    <v-chip>BIOGRAPHY</v-chip>

                    <v-chip>THRILLER</v-chip>

                    <v-chip>HORROR</v-chip>
                  </v-chip-group>
                </v-card>
      </v-flex>
      <v-flex d-flex xs12 sm6 md3 child-flex>
        <v-card>
          <v-card-title primary class="title justify-center">Key Takeaways</v-card-title>
          <v-card-text class="Coursetext">{{ lorem }}</v-card-text>
        </v-card>
      </v-flex>
      <v-flex d-flex xs12 sm6 md9>
        <v-card style="font-size: 40px !important">
          <v-card-title primary class="title justify-center"
            >Course Overview</v-card-title
          >
          <v-card-text class="Coursetext">{{ lorem }}</v-card-text>
          <v-list-item class="d-flex align-start flex-column">
            <v-list-item-subtitle>1.{{ ul }}</v-list-item-subtitle>
            <v-list-item-subtitle>2.{{ ul }} </v-list-item-subtitle>
            <v-list-item-subtitle>3.{{ ul }} </v-list-item-subtitle>
          </v-list-item>
        </v-card>
      </v-flex>
      <v-flex d-flex xs12 sm6 md8>
        <v-img class="img" width="1000">
          <LazyYoutube
            ref="lazyVideo"
            src="https://www.youtube.com/watch?v=8eCoSsTNzG4"
            max-width="1000"
            max-height="500"
            aspect-ratio="16:9"
            thumbnail-quality="standard"
          />
        </v-img>
      </v-flex>
      <v-flex d-flex xs12 sm6 md4>
        <v-card>
          <v-card-title primary class="title justify-center"
            >Is this EMC for you?</v-card-title
          >
          <v-card-text class="Coursetext">{{ lorem }}</v-card-text>
          <v-card-text class="Coursetext">{{ lorem }}</v-card-text>
        </v-card>
      </v-flex>
      <v-flex d-flex xs12 sm6 md4>
        <v-card>
          <v-card-title primary class="title justify-center"
            >About this Mentor</v-card-title
          >
          <v-card-text class="Coursetext">{{ lorem }}</v-card-text>
          <v-card-text class="Coursetext">{{ lorem }}</v-card-text>
          <v-card-text class="Coursetext">{{ lorem }}</v-card-text>
        </v-card>
      </v-flex>
      <v-flex d-flex xs12 sm6 md8>
        <v-card>
          <v-card-title primary class="title justify-center"
            >Why ‘Experiential Micro-Course’?</v-card-title
          >
          <v-card-text class="Coursetext">{{ lorem }}</v-card-text>
          <v-list-item class="d-flex align-start flex-column">
            <v-list-item-subtitle>1.{{ ul }}</v-list-item-subtitle>
            <v-list-item-subtitle>2.{{ ul }} </v-list-item-subtitle>
            <v-list-item-subtitle>3.{{ ul }} </v-list-item-subtitle>
          </v-list-item>
          <v-card-text class="Coursetext">{{ lorem }}</v-card-text>
          <v-list-item class="d-flex align-start flex-column">
            <v-list-item-subtitle>1.{{ ul }}</v-list-item-subtitle>
            <v-list-item-subtitle>2.{{ ul }} </v-list-item-subtitle>
            <v-list-item-subtitle>3.{{ ul }} </v-list-item-subtitle>
          </v-list-item>
          <v-card-text class="Coursetext">{{ lorem }}</v-card-text>
          <v-list-item class="d-flex align-start flex-column">
            <v-list-item-subtitle>1.{{ ul }}</v-list-item-subtitle>
            <v-list-item-subtitle>2.{{ ul }} </v-list-item-subtitle>
            <v-list-item-subtitle>3.{{ ul }} </v-list-item-subtitle>
          </v-list-item>
        </v-card>
      </v-flex>
      <v-flex d-flex xs12 sm12 md12>
        <v-card class="carouselcard">
          <v-card-title primary class="title" style="padding: 3%"
            >Related Experiential Micro-Course</v-card-title
          >
          <carousel class="carousel" />
        </v-card>
      </v-flex>
      <v-flex d-flex grid-list-xl >
        <v-card class="carouselcard">
          <v-card-title primary class="title" style="padding: 3%">
            Related Mentors</v-card-title
          >
          <v-flex>
            <v-layout row wrap>
              <v-flex d-flex xs12 sm6 md3 v-for="i in 4" :key="i">
                <v-card class="Mentors">
                  <v-img
                    class="imgMentors"
                    aspect-ratio="1.7"
                    src="../assets/Screenshotmen.png"
                  >
                  </v-img>
                  <v-card-title
                    primary
                    class="title justify-center"
                    style="color: "
                    >Deepak Shapeti</v-card-title
                  >
                  <v-card-title class="justify-center"
                    >Obsessive Serial Entrepreneur</v-card-title
                  >
                  <v-card-text class="Coursetext justify-center"
                    >{{ lorem.slice(0, 70) }}
                  </v-card-text>
                  <v-chip-group
                    style="margin: 20px"
                    v-model="selection"
                    active-class="red accent-3 white--text"
                    column
                  >
                    <v-chip>BIOGRAPHY</v-chip>

                    <v-chip>THRILLER</v-chip>

                    <v-chip>HORROR</v-chip>
                  </v-chip-group>
                </v-card>
              </v-flex>
            </v-layout>
          </v-flex>
        </v-card>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<style>
@import url("https://fonts.googleapis.com/css2?family=Montserrat:wght@100;400&display=swap");

.v-card {
  border-radius: 32px !important;
  box-shadow: 0px 0px 20px rgba(0, 0, 0, 0.14) !important ;
}

.img {
  border-radius: 32px !important;
  box-shadow: 0px 0px 20px rgba(0, 0, 0, 0.14) !important ;
}

.v-card-title {
  color: rgb(136, 25, 25) !important;
}

.Coursetext {
  font-family: "Montserrat", sans-serif;
  font-weight: 400;
  font-size: 16px !important;
  color: #000 !important ;
}

.carouselcard {
  box-shadow: none !important;
  border-radius: 0px !important;
}

.carousel {
  width: 100vw;
}

.Mentors {
  border-radius: 32px !important;
  height: 800px;
}

.imgMentors {
  border-radius: 32px !important;
  height: 500px;
}

.primaryimg
{
  /* margin-left:20%; */
}

</style>

<script>
import carousel from "../components/carousel";

export default {
  components: {
    carousel,
  },
  data() {
    return {
      lorem: `Digital Marketing 101 is the ultimate primer you need to get started with a career in Digital marketing. 
        This course is a Digital Marketing 101 is the ultimate primer you need to get started with a career in Digital marketing.
        This course isDigital Marketing 101 is the ultimate primer you need to get started.`,
      ul: ` Digital Marketing 101 is the ultimate `,
    };
  },
};
</script>

