<template>
  <nav class="fixed top-5 left-0 right-0 w-full z-70 flex container mx-auto">
    <div
      class="glass-nav h-[58px] border border-white/10 rounded-xl flex justify-between items-center px-3 py-3 w-full transition-transform hover:scale-[1.01] hover:border-primary/80"
    >
      <div class="font-bold cursor-pointer">Yekta</div>

      <button
        class="flex items-center justify-center text-on-surface hover:text-primary transition-colors cursor-pointer"
      >
        <!-- <span class="material-symbols-outlined text-[12px] mr-2">Menu</span> -->
        <svg
          width="32"
          height="32"
          viewBox="0 0 24 24"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
          class="text-primary"
        >
          <path
            d="M4 7L7 7M20 7L11 7"
            stroke="currentColor"
            stroke-width="1.5"
            stroke-linecap="round"
          />
          <path
            d="M20 17H17M4 17L13 17"
            stroke="currentColor"
            stroke-width="1.5"
            stroke-linecap="round"
          />
          <path
            d="M4 12H7L20 12"
            stroke="currentColor"
            stroke-width="1.5"
            stroke-linecap="round"
          />
        </svg>
      </button>
    </div>
  </nav>
</template>

<script lang="ts" setup></script>

<style>
.glass-nav {
  background: rgba(19, 19, 19, 0.4);
  backdrop-filter: blur(32px);
  -webkit-backdrop-filter: blur(32px);
}
</style>
