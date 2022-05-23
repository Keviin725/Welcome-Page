<template>
  <q-layout view="lHh Lpr lFf">
    <q-header elevated>
      <q-toolbar>


        <q-toolbar-title class="font-titulo text-bold">
          Welcome App
        </q-toolbar-title>


      </q-toolbar>
    </q-header>


    <q-footer class="rodape">
      <p class="font-rodape">@Kevin Machava</p>
    </q-footer>
    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>

</script>

<style lang = "scss">
  .rodape{
    text-align: center;

  }
  .font-rodape{
    font-size: 20px;
  }

</style>
