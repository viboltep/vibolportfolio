<template>
    <div class="flex items-center absolute" style="top: 40px; right: 20px;">
        <Icon name="mdi:theme-light-dark" class="me-1" />
        <!-- <h1>Color mode: {{ $colorMode.value }}</h1> -->
        <select v-model="$colorMode.preference" class="rounded-lg bg-white">
            <option value="system">{{ t('home.theme.system') }}</option>
            <option value="light">{{ t('home.theme.light') }}</option>
            <option value="dark">{{ t('home.theme.dark') }}</option>
            
        </select>
       
        
    </div>
</template>

<script setup>

const colorMode = useColorMode()
const {t} = useI18n()
const localePath = useLocalePath()
console.log(colorMode.preference)
</script>

<style>
body {
    background-color: #fff;
    color: rgba(0, 0, 0, 0.8);
}

.dark-mode body {
    background-color: #091a28;
    color: #ebf4f1;
}


</style>