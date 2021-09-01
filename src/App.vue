<template>
  <q-layout view="lHh Lpr lFf">
    <q-header class="bg-white" bordered>
      <div class="container q-pa-sm">
        <div class="row justify-between items-center">
          <div class="col-2">
            <img
              alt="Instagram logo"
              src="@/assets/logo.png"
              style="width: 105px; display: block;"
            >
          </div>
          <div class="col-8 flex items-center justify-end">
            <q-input
              label="pesquisar"
              dense
              filled
              class="mobile-hide"
              style="display: inline-block; margin-right: 150px; width: 200px"
            >
              <template v-slot:prepend>
                <q-icon name="search" />
              </template>
            </q-input>
            <q-btn
              icon="home"
              color="black"
              flat
              padding="sm"
            />
            <q-btn
              icon="o_maps_ugc"
              color="black"
              flat
              padding="sm"
            />
            <q-btn
              icon="o_explore"
              color="black"
              flat
              padding="sm"
            />
            <q-btn
              icon="o_favorite_border"
              color="black"
              flat
              padding="sm"
            />
            <q-avatar size="25px" class="q-ml-sm">
              <img src="https://cdn.quasar.dev/img/avatar4.jpg">
            </q-avatar>
          </div>
        </div>
      </div>
    </q-header>

    <q-page-container class="bg-grey-3">
      <div class="container q-pa-sm">
        <HelloWorld />
      </div>
    </q-page-container>
  </q-layout>
</template>

<script>
import { ref } from 'vue'
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'LayoutDefault',

  components: {
    HelloWorld
  },

  setup () {
    return {
      leftDrawerOpen: ref(false)
    }
  }
}
</script>

<style scoped>
  .container {
    box-sizing: border-box;
    margin: 0 auto;
    max-width: 935px;
  }
</style>
