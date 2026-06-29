<script setup lang="ts">
</script>
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
      <div class="flex justify-center mt-20">
        <button class="feh-shiny-button">
          <div class="feh-border-mask">
            <div class="feh-border-glow"></div>
          </div>
          <span class="">Show More  </span>

        </button>
      </div>
    </div>
  </section>
</template>

<style scoped>
.feh-shiny-button {
  position: relative;
  padding: 10px 30px;
  border-radius: 12px;
  color: #fff;
  font-size: 16px;
  font-weight: 500;
  text-decoration: none;
  background: #1F1F1F;
  transition: all 0.3s ease;
}
.feh-shiny-button:hover {
  background: #333;
}
.feh-border-mask {
  position: absolute;
  top: 0;
  left: 0;
  border-radius: 12px;
  width: 100%;
  height: 100%;
  padding: 1px;
  mask: linear-gradient(#000 0 0) content-box, linear-gradient(#000 0 0) border-box;
  mask-composite: exclude;
}

.feh-border-glow {
  background: conic-gradient(from 0deg, transparent 0%, var(--primary) 10%, #000, transparent 20%);
  position: absolute;
  top: 50%;
  left: 50%;
  width: 500px;
  height: 500px;
  transform: translate(-50%, -50%);
  transform-origin: 0 0;
  animation: rotateShine 3s linear infinite;

}
@keyframes rotateShine {
  0% {
    transform: rotate(0deg) translate(-50%, -50%);
  }
  100% {
    transform: rotate(360deg) translate(-50%, -50%);
  }
}


</style>
