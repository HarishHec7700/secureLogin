<template>
  <section>
    <div
      class="container is-full-height is-flex is-justify-content-center is-align-items-center"
    >
      <section class="login border white radius bg-default my-4 columns">
        <div class="left column bg-pri">
          <h1 class="is-text-9 has-text-weight-bold">Login</h1>
          <q-input
            square
            filled
            v-model="email"
            :label="$t('login.email')"
            class="my-3"
          />
          <q-input
            square
            filled
            v-model="password"
            :label="$t('login.password')"
            class="mb-3"
            type="password"
          />
        </div>
        <div class="right column bg-sec">Hola</div>
      </section>
    </div>
  </section>
</template>

<script setup>
import { ref } from "vue";

const email = ref("");
const password = ref("");
</script>

<style lang="scss" scoped>
.login {
  width: 70%;
}
</style>
