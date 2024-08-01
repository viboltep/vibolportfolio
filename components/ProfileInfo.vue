<template>
    <div class="bg-purple-200 text-center h-screen">
        <h2 class="text-3xl font-bold pt-5 pb-5">{{ t('home.features.title') }}</h2>
      <p>
        {{ t('footer.underlicense') }}
        
      </p>
      <div class="flex mb-4 ">
        
        <div class="w-1/2 h-5/6 bg-white rounded-2xl">
            <h3>Personal Information</h3>
        </div>
       

      </div>
      
    </div>
  </template>
  
  <script setup lang="ts">
  
  const { t } = useI18n();
  </script>
  