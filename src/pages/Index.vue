<template>
  <q-page>
    <div class="row">
      <div class="col bg-primary shadow-10 rounded-borders">
        <h3 class="text-white text-center text-weight-bold">Desarrollador Front-end</h3>
      </div>
    </div>
    <div class="flex flex-center">
      <img class="q-pa-lg" src="~assets/web-design.jpg" alt="Web desing" height="300" width="400">
    </div>
    <div class="row justify-center">
      <div class="col-6">
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Eius ad sed placeat maxime distinctio. Commodi inventore voluptatibus quas architecto, porro, aliquam quae itaque nobis blanditiis exercitationem alias tempora impedit laboriosam!
        </p>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Eius ad sed placeat maxime distinctio. Commodi inventore voluptatibus quas architecto, porro, aliquam quae itaque nobis blanditiis exercitationem alias tempora impedit laboriosam!
        </p>
      </div>
    </div>
    
    <div class="row q-py-xl" >
      <div class="row justify-center bg-teal-13 q-py-md shadow-10 bordes-redon">
        <div class="col text-center contendor">
          <q-icon name="business" class="text-dark mover" />
          <h5 class="text-white text-weight-bold">Sitios Corporativos</h5>
          <p class="text-left q-mx-md text-white">Lorem ipsum dolor sit amet consectetur adipisicing elit. Est, animi corrupti! Autem modi animi incidunt nihil ipsa, odio ullam. Odio porro, exercitationem dolor natus repellat numquam beatae dolorum illo sint?</p>
        </div>
        <div class="col text-center contendor">
          <q-icon name="home" class="text-dark mover" />
          <h5 class="text-white text-weight-bold">Landing page</h5>
          <p class="text-left q-mx-md text-white">Lorem ipsum dolor sit amet consectetur adipisicing elit. Est, animi corrupti! Autem modi animi incidunt nihil ipsa, odio ullam. Odio porro, exercitationem dolor natus repellat numquam beatae dolorum illo sint?</p>
        </div>
        <div class="col text-center contendor">
          <q-icon name="shopping_cart" class="text-dark mover"/>
          <h5 class="text-white text-weight-bold">Tiendas Virtuales</h5>
          <p class="text-left q-mx-md text-white">Lorem ipsum dolor sit amet consectetur adipisicing elit. Est, animi corrupti! Autem modi animi incidunt nihil ipsa, odio ullam. Odio porro, exercitationem dolor natus repellat numquam beatae dolorum illo sint?</p>
        </div>
        <div class="col text-center contendor">
          <q-icon name="desktop_windows" class="text-dark mover" />
          <h5 class="text-white text-weight-bold">Sistemas Web</h5>
          <p class="text-left q-mx-md text-white">Lorem ipsum dolor sit amet consectetur adipisicing elit. Est, animi corrupti! Autem modi animi incidunt nihil ipsa, odio ullam. Odio porro, exercitationem dolor natus repellat numquam beatae dolorum illo sint?</p>
        </div>
      </div>
    </div>
  </q-page>
</template>

<script>
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'PageIndex'
})
</script>

<style lang="scss" scoped>
.bordes-redon{
  border-radius: 20px;
}
.mover{
  position: relative;
  transform: translateY(-25px);
  z-index: 1;
  font-size: 70px;
  height: 0;
}
.contenedor{
  position: absolute;
  z-index: 0;
}
</style>
