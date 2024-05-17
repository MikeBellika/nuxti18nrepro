<script setup lang="ts">
const { setLocale, locale } = useI18n();
function switchLanguage() {
  setLocale(locale.value == 'en' ? 'fr' : 'en');
}
</script>
<template>
  <div>
    {{ $t('welcome') }}
    <button @click="switchLanguage">Switch language</button>
  </div>
</template>
