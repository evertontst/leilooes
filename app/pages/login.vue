<script lang="ts" setup>
import { useSession } from 'h3'

const { loggedIn, user, session, fetch, clear } = useUserSession()

definePageMeta({
  middleware: 'guest',
  layout: 'auth',
})

const title = 'Login'
const description = 'Use one of the following providers to login to your account.'

useSeoMeta({
  title,
  description,
})

const message = useState<string>('message')
if (import.meta.server) {
  const session = await useSession(useRequestEvent()!, {
    password: useRuntimeConfig().session.password,
  })

  message.value = session.data.message

  await session.update({
    message: '',
  })
}
</script>

<template>
  <div v-if="loggedIn">
    <h1>Welcome {{ user.login }}!</h1>
    <p>Logged in since {{ session.loggedInAt }}</p>
    <button @click="clear">
      Logout
    </button>
  </div>
  <div v-else>
    <h1>Not logged in</h1>
    <a href="/auth/google">Login with Google</a>
  </div>
</template>
