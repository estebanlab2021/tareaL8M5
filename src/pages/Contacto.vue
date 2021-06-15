<template>
  <q-page>
    <div class="row">
        <div class="col shadow-10 rounded-borders bg-primary">
        <h3 class="text-white text-center text-weight-bold">Contacto</h3>
    </div>
    </div>

    <div class="row justify-center q-pa-md">
        <div class="col-4 text-center rounded-borders bordes-internos q-pa-md">
            <div class="q-gutter-md" style="max-width: 300px">
                <q-input filled v-model="name" label="Ingrese su nombre" />
                <q-input filled type="email" v-model="email" label="Ingrese su email" hint="Email valid" />
            </div>
            <q-btn  class="q-mt-md" color="positive" glossy label="Enviar" @click="mostrar=true" />
            <q-btn  class="q-mt-md q-ml-lg" color="negative" glossy label="Borrar" @click="Borrar" />
        </div>
    </div>

    <div class="row justify-center">
        <div class="col-6">
            <q-card flat bordered class="q-mt-md bg-grey-2" v-show="mostrar">
                <q-card-section class="row q-gutter-sm items-center">
                  <div class="text-center">Se han ingresado los sigientes datos: {{name}} - {{email}}</div>
                </q-card-section>
                <q-separator />
                <q-card-section>Lo contactaremos en los próximos días. Muchas Gracias!!</q-card-section>
            </q-card>
        </div>
    </div>

  </q-page>
</template>

<script>
import { ref } from 'vue'

export default {
    setup () {
        let mostrar= ref(false);
    return {
      name: ref(''),
      email: ref(''),
      mostrar
    }
  },
  methods: {
      Borrar() {
        this.mostrar = false;
        this.name= '';
        this.email= '';
      }
  },

}
</script>

<style lang="scss" scoped>

.bordes-internos{
  border: 1px solid black;
}

</style>