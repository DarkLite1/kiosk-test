<template>
  <q-page>
    <div class="q-pa-md col-8 q-gutter-md">
      <h4 class="q-mb-xs">{{ $t('page.help.title.hereToHelp') }}</h4>
      <p class="col-12">{{ $t('page.help.paragraph.intro') }}</p>
    </div>

    <div class="row justify-center q-gutter-md text-black">
      <q-card class="my-card bg-secondary" flat bordered>
        <q-card-section horizontal>
          <q-icon class="col-2" size="80px" name="help_outline" />
          <q-card-section>
            <div class="text-h6">{{ $t('page.help.contact1.title') }}</div>
            <div class="text-subtitle2">
              <p>{{ $t('page.help.contact1.intro') }}</p>
              <ul class="q-mb-none">
                <li>
                  <b>{{ $t('page.help.contact1.person.name') }} </b><br />
                  {{ $t('page.help.contact1.person.jobTitle') }}<br />
                  <q-icon name="local_phone" />
                  {{ $t('page.help.contact1.person.phone') }}<br />
                  <q-icon name="mail" />
                  {{ $t('page.help.contact1.person.email') }}
                </li>
              </ul>
            </div>
          </q-card-section>
        </q-card-section>
      </q-card>

      <q-card class="my-card bg-secondary" flat bordered>
        <q-card-section horizontal>
          <q-icon class="col-2" size="80px" name="support_agent" />
          <q-card-section>
            <div class="text-h6">{{ $t('page.help.contact2.title') }}</div>
            <div class="text-subtitle2">
              <p>{{ $t('page.help.contact2.intro') }}</p>
              <ul class="q-mb-none">
                <li>
                  <b>{{ $t('page.help.contact2.person.name') }} </b><br />
                  {{ $t('page.help.contact2.person.jobTitle') }}<br />
                  <q-icon name="local_phone" />
                  {{ $t('page.help.contact2.person.phone') }}<br />
                  <q-icon name="mail" />
                  {{ $t('page.help.contact2.person.email') }}
                </li>
              </ul>
            </div>
          </q-card-section>
        </q-card-section>
      </q-card>
    </div>
  </q-page>
</template>

<script setup lang="ts"></script>

<style scoped>
.my-card {
  width: 100%;
  max-width: 490px;
}
</style>
