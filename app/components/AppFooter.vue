<script lang="ts" setup>
const title = useRuntimeConfig().app.name

const appConfig = useAppConfig()
const notice = appConfig.footer.notice
const smallLinks = appConfig.footer.smallLinks
const socials = appConfig.socials
</script>

<template>
  <footer>footer</footer>
</template>
