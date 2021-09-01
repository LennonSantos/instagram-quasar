<template>
  <q-page>
    <div class="row q-col-gutter-lg">
      <div class="q-mt-lg col-md-8 col-sm-12">
        <q-card flat bordered>
          <q-scroll-area style="height: 110px;">
            <div class="row no-wrap">
              <div v-for="n in 10" :key="n" class="q-pa-sm text-center">
                <q-avatar
                  size="60px"
                  class="q-ma-sm"
                  style="padding: 3px"
                >
                  <img
                    src="https://cdn.quasar.dev/img/avatar.png"
                    style="background: linear-gradient(to right, orange, purple); padding: 3px;"
                  >
                </q-avatar>
                <div style="font-size: 12px">Brunhilde Pan</div>
              </div>
            </div>
          </q-scroll-area>
        </q-card>

        <q-card
          v-for="n in 10" :key="n"
          flat bordered class="q-mt-lg"
        >
          <q-item>
            <q-item-section avatar>
              <q-avatar>
                <img src="https://cdn.quasar.dev/img/avatar2.jpg">
              </q-avatar>
            </q-item-section>

            <q-item-section>
              <q-item-label class="text-weight-bold">maria.doe</q-item-label>
            </q-item-section>

            <q-item-section side>
              <q-btn icon="o_linear_scale" padding="none" flat />
            </q-item-section>
          </q-item>

          <q-separator />

          <q-card-section class="q-pa-none">
            <q-img
              :ratio="1/1"
              src="https://cdn.quasar.dev/img/parallax1.jpg"
            />
          </q-card-section>

          <q-card-section class="q-pa-sm">
            <q-btn
              icon="o_favorite_border"
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
              icon="o_send"
              color="black"
              flat
              padding="sm"
            />
          </q-card-section>

          <q-card-section class="q-pa-sm">
            <q-avatar size="25px" class="q-ml-sm q-mr-sm">
              <img src="https://cdn.quasar.dev/img/avatar4.jpg">
            </q-avatar>
            Curtido por <b>Lennon Bueno</b> e <b>outras 234 pessoas</b>
          </q-card-section>

          <q-card-section class="q-pt-none">
            <div><b>John</b> Eai?</div>
            <div class="text-grey-7">Ver todos os 203 comentários</div>
            <div><b>Maria</b> Que lugar lindo</div>
            <div><b>Pedro</b> Amei</div>
            <div class="text-grey-7">Há 6 horas</div>
          </q-card-section>

          <q-separator />

          <q-item>
            <q-item-section avatar>
              <q-icon name="o_sentiment_satisfied" />
            </q-item-section>

            <q-item-section>
              <q-input
                placeholder="Adicione um comentário"
                dense
                filled
                class="full-width"
                bg-color="white"
              />
            </q-item-section>

            <q-item-section side>
              <q-btn label="Publicar" no-caps color="blue" padding="none" flat />
            </q-item-section>
          </q-item>
        </q-card>
      </div> <!-- .col-8 -->
      <div class="q-mt-lg col-md-4 col-sm-12">
        <q-card flat class="bg-transparent">
          <q-item class="q-mt-md">
            <q-item-section avatar>
              <q-avatar size="50px">
                <img src="https://cdn.quasar.dev/img/avatar4.jpg">
              </q-avatar>
            </q-item-section>

            <q-item-section>
              <q-item-label class="text-weight-bold">bueno.lennon</q-item-label>
              <q-item-label caption>
                Lennon Bueno
              </q-item-label>
            </q-item-section>

            <q-item-section side>
              <q-btn label="Mudar" no-caps color="blue" flat padding="none" />
            </q-item-section>
          </q-item>

          <q-card-section>
            <div class="text-weight-bold text-grey-7">Sugestões para você</div>
          </q-card-section>

          <q-item
            v-for="n in 4" :key="n"
            class="q-mt-sm"
          >
            <q-item-section avatar>
              <q-avatar size="30px">
                <img src="https://cdn.quasar.dev/img/avatar4.jpg">
              </q-avatar>
            </q-item-section>

            <q-item-section>
              <q-item-label class="text-weight-bold">bueno.lennon</q-item-label>
              <q-item-label caption>
                Lennon Bueno
              </q-item-label>
            </q-item-section>

            <q-item-section side>
              <q-btn label="Seguir" no-caps color="blue" flat padding="none" />
            </q-item-section>
          </q-item>
        </q-card>
      </div> <!-- .col-4 -->
    </div> <!-- row -->
  </q-page>
</template>

<style>
</style>

<script>
export default {
  name: 'HelloWorld'
}
</script>
