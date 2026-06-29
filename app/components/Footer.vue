<script lang="ts" setup>
const social = ref([
  {
    title: 'Twitter',
    url: '/twitter',
  },
  {
    title: 'Instagram',
    url: '/twitter',
  },
  {
    title: 'Facebook',
    url: '/twitter',
  },
  {
    title: 'Youtube',
    url: '/twitter',
  },

])
</script>

<template>
  <footer class="border-t border-t-1 border-t-primary/30 py-5">
    <div class="container mx-auto flex justify-center items-center">
      <a
          v-for="(s, i) in social"
          :key="i"
          href=""
          class="mr-5 uppercase opacity-80 text-xs tracking-[0.25em] transition-all duration-300 hover:-translate-y-1 hover:text-primary"
      >
        {{ s.title }}
      </a>
    </div>
  </footer>
</template>

<style scoped>

</style>