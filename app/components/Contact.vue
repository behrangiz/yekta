<script setup lang="ts">
</script>
<template>
  <section class="relative overflow-hidden bg-black py-28">
    <!-- background -->
    <div class="absolute inset-0 bg-black/90 backdrop-blur-3xl"></div>

    <div
        class="absolute -top-40 -right-40 w-[500px] h-[500px] bg-primary/50 blur-[140px] rounded-full float"
    ></div>
    <div
        class="absolute bottom-0 right-0 w-[500px] h-[500px] bg-purple-500/20 blur-[160px] rounded-full float-slow"
    ></div>

    <div class="relative z-10 container mx-auto px-6 pl-20">
      <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 items-center">
        <div class="lg:col-span-1"></div>
        <div class="lg:col-span-5 s">
          <div>
         <span class="text-primary uppercase tracking-[0.35em] text-xs">
            Cotact With Me
          </span>

            <div class="w-20 h-px bg-primary mt-1 mb-2"></div>

            <h2 class="text-4xl lg:text-6xl font-bold leading-tight">
              Building immersive
              <span class="">digital experiences</span>
            </h2>

          </div>
        </div>

        <!-- Content -->
        <div class="lg:col-span-5 pt-10">
          <div class="flex flex-col">
            <label for="">Email</label>
            <input class="bg-gray-50 h-[50px] rounded-lg"/>
          </div>
          <div class="flex flex-col mt-6">
            <label for="">Name</label>
            <input class="bg-gray-50 h-[50px] rounded-lg"/>
          </div>
          <div class="flex flex-col mt-6">
           <button class="w-full h-[50px] rounded-lg bg-primary/20">
             Submit
           </button>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>

</style>
