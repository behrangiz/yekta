<template>
  <section class="relative overflow-hidden bg-black py-28">
    <!-- 
    <div
      class="absolute -top-40 -left-40 w-[500px] h-[500px] bg-primary/30 blur-[140px] rounded-full float"
    ></div>
    <div
      class="absolute bottom-0 right-0 w-[500px] h-[500px] bg-purple-500/20 blur-[160px] rounded-full float-slow"
    ></div> -->
    <div class="relative z-10 container mx-auto">
      <span class="text-primary uppercase tracking-[0.35em] text-xs">
        Latest Projects
      </span>

      <div class="w-20 h-px bg-primary mt-1 mb-2"></div>
      <h2 class="text-4xl lg:text-6xl font-semibold leading-tight">
        Building immersive
        <br />
        <span class="">digital experiences.</span>
      </h2>
    </div>
    <div class="container mx-auto mt-10">
      <div class="grid grid-cols-1 lg:grid-cols-12 gap-8">
        <!-- Left (1/3) -->
        <div class="lg:col-span-6 flex flex-col gap-8">
          <ProjectCard />
        </div>
        <div class="lg:col-span-3">
          <ProjectCard />
        </div>
        <div class="lg:col-span-3">
          <ProjectCard />
        </div>
      </div>
      <div>
        <button class="show-more-btn">
          <span>Show More</span>
        </button>
      </div>
    </div>
  </section>
</template>

<style scoped></style>
