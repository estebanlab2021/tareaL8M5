<template>
  <q-page>
    <div class="row">
        <div class="col bg-primary shadow-10 rounded-borders">
            <h3 class="text-white text-center text-weight-bold">Servicios que ofrecemos</h3>
        </div>
    </div>
    
    <div class="row justify-center">
        <div class="col-4 q-pa-md q-gutter-md">
            <q-card class="my-card" >
                <q-img src="~assets/computadora.jpg">
                  <div class="absolute-bottom">
                    <div class="text-h6">DISEÑO DE PÁGINAS WEB</div>
                    <div class="text-subtitle2">Subtitle</div>
                  </div>
                </q-img>
                <q-card-section>Un texto</q-card-section>
                <q-card-actions class="row justify-center" >
                  <q-btn flat glossy @click="alerta = true">Más Información</q-btn>
                </q-card-actions>
            </q-card>
        </div>
        <div class="col-4 q-pa-md q-gutter-md">
            <q-card class="my-card" >
                <q-img src="~assets/code.jpg">
                  <div class="absolute-bottom">
                    <div class="text-h6">DISEÑOS WEB PERSONALIZADOS</div>
                    <div class="text-subtitle2">Subtitle</div>
                  </div>
                </q-img>
                <q-card-section>Un texto</q-card-section>
                <q-card-actions class="row justify-center" >
                  <q-btn flat glossy @click="alerta = true">Más Información</q-btn>
                </q-card-actions>
            </q-card>
        </div>
        <div class="col-4 q-pa-md q-gutter-md">
            <q-card class="my-card" >
                <q-img src="~assets/website.jpg">
                  <div class="absolute-bottom">
                    <div class="text-h6">DISEÑOS MODERNOS Y CONFIABLES</div>
                    <div class="text-subtitle2">Subtitle</div>
                  </div>
                </q-img>
                <q-card-section>Un texto</q-card-section>
                <q-card-actions class="row justify-center" >
                  <q-btn flat glossy @click="alerta = true">Más Información</q-btn>
                </q-card-actions> 
            </q-card>
        </div>
    </div>
    <q-dialog v-model="alerta">
        <q-card>
          <q-card-section>
            <div class="text-h6">Más Información</div>
          </q-card-section>

          <q-card-section class="q-pt-none">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Rerum repellendus sit voluptate voluptas eveniet porro. Rerum blanditiis perferendis totam, ea at omnis vel numquam exercitationem aut, natus minima, porro labore.
          </q-card-section>

          <q-card-actions align="right">
            <q-btn flat label="OK" color="primary" v-close-popup />
          </q-card-actions>
        </q-card>
      </q-dialog>
  </q-page>
</template>

<script>
import { ref } from 'vue'

export default {
    setup(){
        return{
            alerta: ref(false)
        }
    }

}
</script>

<style>

</style>