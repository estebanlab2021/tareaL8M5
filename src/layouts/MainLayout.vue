<template>
  <div class="q-pa-md">
    <q-layout view="lHh Lpr lff" >
      <q-header elevated class="bg-cyan-8">
        <q-toolbar>
          <q-toolbar-title>Header</q-toolbar-title>
          <div>Quasar v{{ $q.version }}</div>
          <q-btn flat @click="drawer = !drawer" round dense icon="menu" />
        </q-toolbar>
      </q-header>

      <q-drawer
        v-model="drawer"
        show-if-above
        :width="200"
        :breakpoint="400"
      >
        <q-scroll-area style="height: calc(100% - 150px); margin-top: 150px; border-right: 1px solid #ddd">
          <q-list padding> 

            <q-item clickable v-ripple to="/" active-class="my-menu-link" exact>
              <q-item-section avatar>
                <q-icon name="home" />
              </q-item-section>

              <q-item-section>
                Inicio
              </q-item-section>
            </q-item>

            <q-item clickable v-ripple to="/about" active-class="my-menu-link">
              <q-item-section avatar>
                <q-icon name="star" />
              </q-item-section>

              <q-item-section>
                Nosotros
              </q-item-section>
            </q-item>

            <q-item clickable v-ripple to="/servicios" active-class="my-menu-link">
              <q-item-section avatar>
                <q-icon name="send" />
              </q-item-section>

              <q-item-section>
                Servicios
              </q-item-section>
            </q-item>

            <q-item clickable v-ripple to="/contacto" active-class="my-menu-link">
              <q-item-section avatar>
                <q-icon name="drafts" />
              </q-item-section>

              <q-item-section>
                Contacto
              </q-item-section>
            </q-item>
          </q-list>
        </q-scroll-area>

        <q-img class="absolute-top" src="https://cdn.quasar.dev/img/material.png" style="height: 150px">
          <div class="absolute-bottom bg-transparent">
            <q-avatar size="56px" class="q-mb-sm">
              <img src="https://cdn.quasar.dev/img/boy-avatar.png">
            </q-avatar>
            <div class="text-weight-bold">Esteban Arroyo</div>
            <div>@estebanlab</div>
          </div>
        </q-img>
      </q-drawer>

      <q-footer elevated>
        <q-toolbar>
          <q-toolbar-title class="text-center">© 2021 | Esteban Arroyo</q-toolbar-title>
        </q-toolbar>
      </q-footer>

      <q-page-container>
        <router-view></router-view>
      </q-page-container>
    </q-layout>
  </div>
</template>

<script>
import { ref } from 'vue'
import { useQuasar } from 'quasar'

export default {
  setup () {
    const drawer = ref(false)
    const $q = useQuasar()

    return {
      drawer,
      $q
    }
  }
}
</script>

<style lang="scss">
.my-menu-link{
  color: white;
  background: #f2c037;
}
</style>