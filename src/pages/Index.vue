<template>
  <q-page class="container" padding>


    <q-form @submit.prevent.stop="onSubmit">
      <q-input rounded clear-icon="close" clearable outlined v-model="form.nome" color="primary" label="Escreva o nome" class="col-md-12 col-sm-12 col-xs-12" :rules="[val => val && val.length > 0 || 'Preencha o formulario']">

        <template v-slot:prepend>
          <q-icon name="person"></q-icon>
        </template>

      </q-input>


    </q-form>


    <q-btn class="botao" label="Submeter" type="submit" rounded color="primary" padding @click="onSubmit()">

    </q-btn>

  </q-page>
</template>

<script>


export default {
  name: 'PageIndex',
  data (){
    return{
      form: {
        nome: " "
      }

    }
  },
  methods:{
    onSubmit(){
      this.$q.dialog({
        title: 'Welcome',
        message: ("Bem vindo "+this.form.nome)

      })
    }
  }


}
</script>

<style lang="scss">
  .botao{
    margin-top: 15px;
  }
</style>
