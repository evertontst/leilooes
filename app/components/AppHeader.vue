<script lang="ts" setup>
// const { $csrfFetch } = useNuxtApp()

// const { loggedIn, session, user } = useUserSession()

// const items = [
//   [
//     {
//       label: 'Profile',
//       to: '/profile',
//       icon: 'i-ph-user-duotone',
//     },
//   ],
//   [
//     {
//       label: 'Logout',
//       icon: 'i-ph-sign-out-duotone',
//       click: async () => {
//         await $csrfFetch('/api/_auth/session', {
//           method: 'DELETE',
//         })

//         session.value = {}

//         await navigateTo('/')
//       },
//     },
//   ],
// ]

// const title = useRuntimeConfig().app.name
// const icon = useAppConfig().app.logo
</script>

<template>
  <header class="navbar">
    <div class="container flex wrap items-center justify-between w-full mt-0 mx-auto">
      <div class="logo">
        Leilõões
      </div>
      <nav>
        <ul class="flex flex-row gap-6">
          <li>
            <NuxtLink to="/">
              Leilões
            </NuxtLink>
          </li>
          <li>
            <NuxtLink to="/">
              Funcionalidades
            </NuxtLink>
          </li>
          <li>
            <NuxtLink to="/">
              Entre em contato
            </NuxtLink>
          </li>
        </ul>
      </nav>
      <NuxtLink to="login">
        Entrar
      </NuxtLink>
    </div>
  </header>
</template>

<style>
header {
  width: 100%;
  height: 75px;
  position: relative;
  background: #121519;
  color:#fff;
  padding: 12px 0;
  z-index: 999;
  -webkit-box-shadow: 0 24px 41px rgba(0, 0, 0, .1),
  0 9px 22px rgba(0, 0, 0, .06) !important;
  box-shadow: 0 4px 21px rgba(0, 0, 0, .03),
  0 9px 12px rgba(0, 0, 0, .01) !important;
}
@media (min-width: 1400px) {
  .container {
    max-width: 1328px;
  }
}
button {
  position: relative;
  background: #448c74;
  color: #fff;
  padding: 12px 30px;
  border-radius: 100px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  border: 2px solid #448c74;
}
</style>
