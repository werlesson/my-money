<template>
  <vs-navbar v-model="active" center-collapsed>
    <template #left>
      <!-- LOGO -->
      <!-- <img src="/logo2.png" alt=""> -->
    </template>
    <vs-navbar-item id="guide" :active="active == 'guide'">
      Guide
    </vs-navbar-item>
    <vs-navbar-item id="docs" :active="active == 'docs'">
      Documents
    </vs-navbar-item>
    <vs-navbar-item id="components" :active="active == 'components'">
      Components
    </vs-navbar-item>
    <vs-navbar-item id="license" :active="active == 'license'">
      license
    </vs-navbar-item>
    <template #right>
      <vs-button flat>Login</vs-button>
      <vs-button>Get Started</vs-button>
    </template>
  </vs-navbar>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'
@Component
export default class Navbar extends Vue {
  active: string = 'guide'
}
</script>
