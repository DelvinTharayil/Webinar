<template>
  <v-app>
    <v-main>
      <WebinarHome/>
    </v-main>
  </v-app>
</template>

<script>
import WebinarHome from './components/WebinarHome';

export default {
  name: 'App',

  components: {
    WebinarHome,
  },

  data: () => ({
    //
  }),
};
</script>
