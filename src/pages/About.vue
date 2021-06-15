<template>
  <q-page>
    <div class="row">
      <div class="col shadow-10 rounded-borders bg-primary">
        <h3 class="text-white text-center text-weight-bold">Sobre Nosotros</h3>
      </div>
    </div>
    <div class="flex flex-center">
      <img class="q-pa-lg" src="~assets/nosotros.jpg" alt="Web desing" height="300" width="400">
    </div>
    <div class="row justify-center items-center">
      <div class="col-4">
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatem, rem sit consectetur ipsum voluptate dignissimos nam soluta similique distinctio quas nisi numquam atque ut excepturi non aut sequi a quia.</p>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatem, rem sit consectetur ipsum voluptate dignissimos nam soluta similique distinctio quas nisi numquam atque ut excepturi non aut sequi a quia.</p>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatem, rem sit consectetur ipsum voluptate dignissimos nam soluta similique distinctio quas nisi numquam atque ut excepturi non aut sequi a quia.</p>
      </div>
      <div class="col-4">
        <img class="q-pa-lg" src="~assets/nosotros2.jpg" alt="Web desing" height="350" width="450">
      </div>
    </div>
    <div class="row justify-center">
      <div class="col-6">
        <h4 class="text-center">Nuestros valores</h4>
        <div class="row justify-center">
          <div class="col-5">
            <q-list dense bordered padding class="rounded-borders" style="max-width: 400px">
              <q-item clickable v-ripple>
                <q-item-section>
                  Item
                </q-item-section>
              </q-item>
              <q-item clickable v-ripple>
                <q-item-section>
                  Item
                </q-item-section>
              </q-item>
              <q-item clickable v-ripple>
                <q-item-section>
                  Item
                </q-item-section>
              </q-item>
              <q-item clickable v-ripple>
                <q-item-section>
                  Item
                </q-item-section>
              </q-item>
              <q-item clickable v-ripple>
                <q-item-section>
                  Item
                </q-item-section>
              </q-item>
            </q-list>
          </div>
        </div>
      </div>
      <div class="col-6">
        <h4 class="text-center">Nuestro Equipo</h4>
        <q-list bordered padding style="max-width: 400px">
          <q-item clickable v-ripple>
              <q-item-section avatar>
                <q-avatar rounded>
                  <img src="https://cdn.quasar.dev/img/boy-avatar.png">
                </q-avatar>
              </q-item-section>
              <q-item-section>
                <q-item-label>Ned Flanders</q-item-label>
                <q-item-label caption>Presidente</q-item-label>
              </q-item-section>
          </q-item>
          <q-item clickable v-ripple>
              <q-item-section avatar>
                <q-avatar rounded>
                  <img src="https://cdn.quasar.dev/img/boy-avatar.png">
                </q-avatar>
              </q-item-section>
              <q-item-section>
                <q-item-label>Homero Simpson</q-item-label>
                <q-item-label caption>Director de Finanzas</q-item-label>
              </q-item-section>
          </q-item>
          <q-item clickable v-ripple>
              <q-item-section avatar>
                <q-avatar rounded>
                  <img src="https://cdn.quasar.dev/img/boy-avatar.png">
                </q-avatar>
              </q-item-section>
              <q-item-section>
                <q-item-label>Seymour Skinner</q-item-label>
                <q-item-label caption>Jefe de Desarrollo Web</q-item-label>
              </q-item-section>
          </q-item>
        </q-list>
      </div>
    </div>
    <div class="flex flex-center q-py-lg"> <!-- height="200" width="200" -->
      <q-btn to="/contacto">
        <q-avatar size="200px">
          <img src="~assets/contacto.png" alt="contacto" >
        </q-avatar>
      </q-btn> 
      
    </div>
  </q-page>
</template>

<script>
export default {

}
</script>

<style>

</style>