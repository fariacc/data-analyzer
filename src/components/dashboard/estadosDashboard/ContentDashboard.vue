<template>
  <div class="content-dashboard pb-2 bg-cinza">
    <div class="row content mx-3 box-shadow">
      <grafico-dashboard></grafico-dashboard>
      <div class="col-sm-12 col-md-12 col-lg-6">
        <info-estados-dashboard :opcao="opcao"></info-estados-dashboard>
      </div>
    </div>
  </div>
</template>

<script>
  import GraficoDashboard from './GraficoDashboard.vue'
  import InfoEstadosDashboard from './InfoEstadosDashboard.vue'
  export default {
    name: 'content-dashboard',
    components: { GraficoDashboard, InfoEstadosDashboard },
    props: { opcao: String }
  }
</script>

<style lang="scss">
  .content-dashboard{
    .content{
      background-color: #ffffff;
      border-radius: 3px;
    }
  }
</style>
