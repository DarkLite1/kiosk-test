<template>
  <q-page>
    <div class="q-pa-md col-8 q-gutter-md">
      <h4 class="q-mb-xs">{{ $t('page.shortcuts.title.quickAccess') }}</h4>
      <p class="col-12">{{ $t('page.shortcuts.paragraph.intro') }}</p>
    </div>

    <div class="q-pa-md" style="max-width: 350px">
      <q-list bordered separator dark>
        <q-item
          v-ripple
          href="https://apps.mypurecloud.de/directory/#/analytics/dashboards/"
          target="_blank"
          clickable
        >
          <q-item-section avatar>
            <q-avatar>
              <img src="/img/GenesysCloud.svg" />
            </q-avatar>
          </q-item-section>
          <q-item-section>{{
            $t('page.shortcuts.button.genesysCloud')
          }}</q-item-section>
        </q-item>
        <q-item
          v-ripple
          href="https://hmnl.inbisco.nl/PM/c208fa1d-31ba-45a0-8122-3ece29b3a38c"
          target="_blank"
          clickable
        >
          <q-item-section avatar>
            <q-avatar>
              <img src="/img/Inbisco.png" />
            </q-avatar>
          </q-item-section>
          <q-item-section>{{
            $t('page.shortcuts.button.inbisco')
          }}</q-item-section>
        </q-item>
      </q-list>
    </div>
  </q-page>
</template>

<script setup lang="ts"></script>
