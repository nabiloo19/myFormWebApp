<template>
  <v-container>
    <v-layout text-center wrap>
      <v-flex xs12>

        <v-form
          ref="form"
          class="mt-4"
          style="text-align:center;"
          action="https://docs.google.com/forms/u/0/d/e/1FAIpQLScAwAVrcoO26ozOjlt0FihaKst25Jy__cYGVmVuSuk8sM1PhQ/formResponse"
          target="_blank"
          method="POST"
          id="mG61Hd"
          >
          
          <v-text-field
            name="entry.1267155872"
            id="name"
            prepend-inner-icon="mdi-account"
            v-model="name"
            label="Name"
            :rules="nameRules"
            outlined
            shaped
            hint="Enter Your Name"
            clearable
            required
            color="purple"
            type="text"
          ></v-text-field>

          <v-text-field
          name="entry.1835978739"
            prepend-inner-icon="mdi-email"
            id="email"
            v-model="email"
            :rules="emailRules"      
            label="Email"
            hint="For example, abc@gmail.com"
            clearable
            required
            color="purple"
            type="text"
            outlined
            shaped
          ></v-text-field>

          <v-text-field
            name="entry.530032414"
            prepend-inner-icon="mdi-phone"
            id="phone"
            :v-model="{phone}"
            :rules="phoneRules"            
            label="Phone Number"
            hint="For example, 123 456 789"
            clearable
            required
            color="purple"
            prefix="+251 "
            outlined
            shaped
          ></v-text-field>

          <v-textarea
          name="entry.2104863854"
            id="message"
            v-model="message"            
            label="Your Message"
            hint="Write Down Your Thoughts and we'll get to you"
            outlined
            shaped
            clearable
            auto-grow
            counter="400"
            color="purple"
            type="text"
          ></v-textarea>

          <v-btn
            class="mr-4 elevation-5"
            type="submit"
            @click="validate"
          >Submit</v-btn>

          <v-btn class="mr-4 elevation-5" @click="reset">Reset Form</v-btn>
        </v-form>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>

export default {

  name: "Form",

  data: () => ({

    name: "",
    email: "",
    message: "",
    phone: "",

    nameRules: [v => !!v || "Name is required"],
    phoneRules: [v => !!v || "Number is required"],
    emailRules: [
      v => !!v || 'E-mail is required',
      v => /^\w+([.-]?\w+)*@\w+([.-]?\w+)*(\.\w{2,3})+$/.test(v) || 'E-mail must be valid'
    ]
    
  }),

  methods: {
    validate() {
      this.$refs.form.validate();
    },
    reset() {
      this.$refs.form.reset();
    }
  }
};
</script>

          id="mG61Hd"
          action="https://docs.google.com/forms/u/0/d/e/1FAIpQLScuIMzoY86m7b2SKW9PvynR5wAJEeSfc9kNoqbdEsTygnhq3Q/formResponse"
          target="_blank"
          method="POST"

          name="entry.1429357351"
          name="entry.1429569306"
          name="entry.925247241"
          name="entry.1838964298"