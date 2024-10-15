<template>
  <q-layout view="hHh lpr fFf" class="lexend bg-image text-white">
    <q-header elevated class="row q-pt-md" height-hint="98">
      <q-toolbar class="col-6">
        <q-toolbar-title>
          <q-img
            src="/img/HeidelbergMaterials.svg"
            alt="Heidelberg Materials"
          />
        </q-toolbar-title>
      </q-toolbar>
    </q-header>

    <q-page-container>
      <div class="row justify-center">
        <router-view />
      </div>
    </q-page-container>

    <q-footer elevated>
      <q-toolbar>
        <div class="text-italic text-weight-thin">
          {{ $t('footer.slogan') }}
        </div>
        <q-toolbar-title />
        <q-select
          v-model="locale"
          :options="localeOptions"
          :label="$t('footer.language')"
          dark
          dense
          outlined
          emit-value
          map-options
          options-dense
          options-selected-class="text-white text-bold"
          style="min-width: 135px"
        />
      </q-toolbar>
    </q-footer>
  </q-layout>
</template>

<script setup lang="ts">
import { useI18n } from 'vue-i18n'
import { ref } from 'vue'

const { locale } = useI18n({ useScope: 'global' })

const localeOptions = ref([
  { value: 'en-US', label: 'English' },
  { value: 'nl-BE', label: 'Nederlands' },
  { value: 'fr-BE', label: 'Francais' },
])
</script>

<style>
.bg-image {
  background-image: url('/img/Background.png');
  background-repeat: no-repeat;
  background-size: cover;
}
</style>
