<script lang="ts" setup>
useHead({
  titleTemplate: title => title ? `${title} - Leilõões` : 'Leilõões',
})
</script>

<template>
  <div>
    <NuxtRouteAnnouncer />
    <NuxtLayout>
      <NuxtPage />
    </NuxtLayout>
  </div>
</template>
