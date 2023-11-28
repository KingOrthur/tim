<template>
  <div id="app">
    <logreg-header v-if="$route.name === 'login'"/>
    <logreg-header v-else-if="$route.name === 'register'"/>

    <app-header v-else-if="$route.name !== 'login'"/>

    <logreg-footer v-if="$route.name === 'login'"/>
    <logreg-footer v-else-if="$route.name === 'register'"/>

  </div>
  <RouterView />
</template>


<script>
import AppHeader from '@/components/App/app-header.vue'
import LogregHeader from '@/components/Logreg/logreg-header.vue'
import LogregFooter from '@/components/Logreg/logreg-footer.vue'


export default {
  components: { AppHeader, LogregHeader, LogregFooter},
}
</script>







<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
