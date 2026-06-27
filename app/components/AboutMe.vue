<template>
  <section class="relative min-h-[700px] overflow-hidden bg-black py-20 mt-20">
    <div class="absolute inset-0 bg-black/60 backdrop-blur-3xl z-0"></div>

    <div
      class="absolute -top-32 -left-32 w-96 h-96 bg-primary/40 blur-3xl rounded-full float"
    ></div>

    <div
      class="absolute top-1/3 -right-32 w-[28rem] h-[28rem] bg-purple-500/30 blur-3xl rounded-full"
    ></div>

    <div
      class="absolute bottom-0 left-1/3 w-96 h-96 bg-cyan-400/20 blur-3xl rounded-full"
    ></div>

    <!-- Content -->
    <div class="container mx-auto">
      <div class="relative z-10 text-white grid grid-cols-2">
        <div
          class="rounded-xl overflow-hidden w-full h-[550px] transition-all hover:border-primary"
        >
          <img
            src="https://plus.unsplash.com/premium_photo-1682146717223-874ac7dcc607?q=80&w=1170&auto=format&fit=crop&ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
            alt=""
            class="grayscale-50 transition-all hover:grayscale-0"
          />
        </div>
        <div class="px-5">
          <h1 class="text-1xl font-bold mt-20">About</h1>
        </div>
      </div>
    </div>
  </section>
</template>

<script lang="ts" setup></script>

<style>
@keyframes float {
  0%,
  100% {
    transform: translateY(0px);
  }
  50% {
    transform: translateY(30px);
  }
}

.float {
  animation: float 8s ease-in-out infinite;
}
</style>
