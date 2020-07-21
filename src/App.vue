<template>
  <div id="app">
    <div class="jumbotron jumbotrom-fluid">
      <div class="container">
        <h1 class="display-4">Vuex</h1>
        <p class="lead">Padrão de gerenciamento de estado</p>
        <Contador/>
      </div>
    </div>
  </div>
</template>


<script>
import Contador from '@/components/Contador.vue'

export default {
  components: {
    Contador
  }
}
</script>