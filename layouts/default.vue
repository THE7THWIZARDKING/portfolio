<template>
  <v-app>
    <NuxtLoadingIndicator />
    <header>
      <Header />
    </header>
    <main>
      <slot />
    </main>
    <Footer />
  </v-app>
</template>
  