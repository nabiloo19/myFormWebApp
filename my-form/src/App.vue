<template>
  <v-app>
    <v-app-bar app dark>
      <div class="d-flex align-center ml-5">
        <span>Form WebApp</span>
      </div>
    </v-app-bar>

    <v-content>
      <Form />
    </v-content>
  </v-app>
</template>

<script>
import Form from "./components/Form";

export default {
  name: "App",

  components: {
    Form
  },

  data: () => ({
    //
  })
};
</script>
