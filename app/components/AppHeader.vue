<script lang="ts" setup>
const { $csrfFetch } = useNuxtApp()

const { loggedIn, session, user } = useUserSession()

const items = [
  [
    {
      label: 'Profile',
      to: '/profile',
      icon: 'i-ph-user-duotone',
    },
  ],
  [
    {
      label: 'Logout',
      icon: 'i-ph-sign-out-duotone',
      click: async () => {
        await $csrfFetch('/api/_auth/session', {
          method: 'DELETE',
        })

        session.value = {}

        await navigateTo('/')
      },
    },
  ],
]

const title = useRuntimeConfig().app.name
const icon = useAppConfig().app.logo
</script>

<template>
  <div>header</div>
</template>
