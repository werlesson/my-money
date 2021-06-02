<template>
  <div class="center examplex">
    <CNavbar />
    <div class="square">
      <Nuxt />
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'
import CNavbar from './navbar/index.vue'

@Component({
  components: {
    CNavbar,
  },
})
export default class TemplateDefault extends Vue {}
</script>
