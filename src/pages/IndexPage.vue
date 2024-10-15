<template>
  <q-page>
    <div class="q-pa-md col-8 q-gutter-md">
      <h4 class="q-mb-xs">{{ $t('page.home.title.safetyCourses') }}</h4>
      <p class="col-12">{{ $t('page.home.paragraph.intro') }}</p>
    </div>

    <div class="row justify-center q-gutter-md q-px-md">
      <q-card class="bg-secondary text-black" style="max-width: 780px">
        <q-card-section>
          <div class="text-h6">
            {{ $t('page.home.title.eLearningTools') }}
          </div>
          <div class="text-subtitle2">
            {{ $t('page.home.paragraph.eLearningTools') }}
          </div>
        </q-card-section>

        <q-card-section class="q-pt-none q-gutter-sm">
          <q-btn
            class="bg-primary text-white q-pl-sm q-pl-sm"
            href="https://wd3-impl.workday.com/wday/authgwy/heidelbergmaterials6/login.htmld?redirect=n"
            target="_blank"
          >
            <div class="q-py-xs">
              <q-avatar round size="2.4em">
                <q-img src="/img/Workday.svg" size="lg" />
              </q-avatar>
            </div>
            <div class="q-pl-sm">{{ $t('page.home.button.workday') }}</div>
          </q-btn>

          <q-btn
            class="bg-primary text-white q-pl-sm q-pl-sm"
            href="https://wd3.myworkday.com/heidelbergmaterials/learning"
            target="_blank"
          >
            <div class="q-py-xs">
              <q-avatar round size="2.4em">
                <q-img src="/img/Workday.svg" size="lg" />
              </q-avatar>
            </div>
            <div class="q-pl-sm">{{ $t('page.home.button.workdaySSO') }}</div>
          </q-btn>

          <q-btn
            class="bg-primary text-white q-pl-sm q-pl-sm"
            href="https://thar.online/login"
            target="_blank"
          >
            <div class="q-py-xs">
              <q-avatar round size="2.4em" class="q-pl-xs">
                <q-img src="/img/Thar.jpg" size="lg" />
              </q-avatar>
            </div>

            <div class="q-pl-md">{{ $t('page.home.button.thar') }}</div>
          </q-btn>

          <q-btn
            class="bg-primary text-white q-pl-sm"
            href="https://gpi.explainsafe.nl"
            target="_blank"
          >
            <q-icon left size="3em" name="task" class="q-mr-xs" />
            <div>{{ $t('page.home.button.gpi') }}</div>
          </q-btn>

          <q-btn
            class="bg-primary text-white q-pl-sm"
            href="https://heidelbergmaterials.learning-service.com/Default"
            target="_blank"
          >
            <q-icon left size="3em" name="school" class="q-mr-sm" />
            <div>{{ $t('page.home.button.fastpass') }}</div>
          </q-btn>

          <q-btn
            class="bg-primary text-white q-pl-sm"
            href="https://heidelbergcement.csod.com/client/heidelbergcement/default.aspx"
            target="_blank"
          >
            <q-icon left size="3em" name="school" class="q-mr-sm" />
            <div>{{ $t('page.home.button.ecampusLogin') }}</div>
          </q-btn>

          <q-btn
            class="bg-primary text-white q-pl-sm"
            href="https://heidelbergcement.csod.com/selfreg/register.aspx?c=hc_contractors"
            target="_blank"
          >
            <q-icon left size="3em" name="school" class="q-mr-sm" />
            <div>{{ $t('page.home.button.ecampusRegister') }}</div>
          </q-btn>

          <q-btn
            class="bg-primary text-white q-pl-sm"
            href="https://poortinstructienetbeheernederland.nl/"
            target="_blank"
          >
            <q-icon left size="3em" name="school" class="q-mr-sm" />
            <div>
              {{ $t('page.home.button.poortinstructiesNetbeheerNederland') }}
            </div>
          </q-btn>
        </q-card-section>
      </q-card>
    </div>

    <div class="row justify-center">
      <h2 class="text-center text-italic q-mb-none q-px-md">
        {{ $t('page.home.title.slogan') }}
      </h2>
    </div>
  </q-page>
</template>

<script setup lang="ts"></script>
