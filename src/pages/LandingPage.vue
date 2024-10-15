<template>
  <q-page>
    <div class="q-pa-md col-8 q-gutter-md">
      <h4 class="q-mb-xs">{{ $t('page.landing.title.selectCountry') }}</h4>
      <p class="col-12">{{ $t('page.landing.paragraph.intro') }}</p>
    </div>

    <div class="row justify-center q-gutter-md text-black">
      <q-card
        v-for="country in $tm('page.landing.countries')"
        :key="country.code"
        class="bg-secondary"
        flat
        bordered
      >
        <q-card-section horizontal>
          <q-card-section>
            <div class="text-h6">
              {{ $rt(country.name) }}
            </div>
          </q-card-section>
        </q-card-section>
      </q-card>
    </div>
  </q-page>
</template>

<script setup lang="ts">
// interface Country {
//   code: string
//   name: string
// }
</script>

<style scoped></style>
