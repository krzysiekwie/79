<template>
  <div class="home">
    <DecadeIndex msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
// @ is an alias to /src
import DecadeIndex from '@/components/DecadeIndex.vue'

export default {
  name: 'home',
  components: {
    DecadeIndex
  }
}
</script>
