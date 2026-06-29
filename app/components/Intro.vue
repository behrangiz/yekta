<template>
  <div class="h-200 relative">
    <div class="absolute right-0 w-4/5 h-full z-10 overflow-hidden">
      <img
        src="/yekta.jpg"
        alt=""
        class="w-full h-full object-cover object-top"
      />
    </div>
    <div
      class="gd bg-linear-to-r from-black/80   to-transparent z-20 w-full h-full absolute"
    ></div>
    <div
      class="container z-20 relative mx-auto w-full h-full flex items-center opacity-90"
    >
      <div>
        <h3 class="text-5xl">Hey,</h3>
        <h1 class="text-8xl font-bold">
          I’m Yekta <span class="">Tabibi</span>
        </h1>
        <p class="mt-2">A cinematographer and director.</p>
      </div>
    </div>
    <div
      class="absolute bottom-0 left-1/2 -translate-x-1/2 flex flex-col items-center gap-4 z-30"
    >
      <span
        class="font-label-caps text-[10px] tracking-[0.4em] rotate-90 origin-left ml-2 opacity-90"
        >SCROLL</span
      >
      <div
        class="scroll-line w-px h-20 bg-linear-to-b from-primary to-transparent"
      ></div>
    </div>
  </div>
</template>

<script lang="ts" setup></script>

<style scoped>
@keyframes scrollLine {
  0% {
    transform: scaleY(0.2);
    opacity: 0.3;
  }
  50% {
    transform: scaleY(1);
    opacity: 1;
  }
  100% {
    transform: scaleY(0.2);
    opacity: 0.3;
  }
}

.scroll-line {
  animation: scrollLine 1.8s ease-in-out infinite;
  transform-origin: top;
}
</style>
