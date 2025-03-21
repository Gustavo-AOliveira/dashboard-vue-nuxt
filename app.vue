<template>
    <v-row style="height: 100vh">
      <v-col class="d-flex flex-column justify-center align-center">
        <v-btn
          v-for="(button, index) in buttons"
          :key="index"
          class="ma-2"
          :color="button.color"
        >
          {{ button.label }}
        </v-btn>
      </v-col>
    </v-row>
  </template>
  
  <script>
  export default {
    data() {
      return {
        buttons: [
          { label: 'Vue', color: 'red' },
          { label: 'Vue Router', color: 'green' },
          { label: 'Vuex', color: 'yellow' },
          { label: 'Vue I18n', color: 'purple' },
          { label: 'Vue Composition API', color: 'orange' },
          { label: 'Vue Devtools', color: 'pink' },
          { label: 'Vue CLI', color: 'teal' },
          { label: 'Vue Test Utils', color: 'cyan' },
          { label: 'Vue SSR', color: 'indigo' },
          { label: 'Vuetify', color: 'blue' },
        ],
      };
    },
  };
  </script>