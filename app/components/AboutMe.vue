<template>
  <section class="relative overflow-hidden bg-black py-28">
    <!-- background -->
    <div class="absolute inset-0 bg-black/70 backdrop-blur-3xl"></div>

    <div
      class="absolute -top-40 -left-40 w-[500px] h-[500px] bg-primary/30 blur-[140px] rounded-full float"
    ></div>
    <div
      class="absolute bottom-0 right-0 w-[500px] h-[500px] bg-purple-500/20 blur-[160px] rounded-full float-slow"
    ></div>

    <!-- content -->
    <div class="relative z-10 container mx-auto px-6">
      <div class="grid grid-cols-1 lg:grid-cols-2 gap-16 items-center">
        <!-- IMAGE -->
        <div class="image-reveal group relative order-2 lg:order-1">
          <div
            class="absolute -inset-2 bg-gradient-to-r from-primary/40 to-purple-500/40 blur-2xl opacity-40 group-hover:opacity-70 transition"
          ></div>

          <div
            class="relative rounded-2xl overflow-hidden border border-white/10"
          >
            <img
              src="https://plus.unsplash.com/premium_photo-1682146717223-874ac7dcc607?q=80&w=1170&auto=format&fit=crop"
              class="w-full h-[420px] md:h-[560px] object-cover grayscale group-hover:grayscale-0 group-hover:scale-110 transition duration-700"
            />
          </div>
        </div>

        <!-- TEXT -->
        <div class="text-reveal text-white order-1 lg:order-2">
          <!-- label -->
          <p class="text-xs tracking-[0.5em] text-primary uppercase opacity-80">
            About Me
          </p>

          <div class="w-16 h-[2px] bg-primary mt-3 mb-6"></div>

          <!-- title -->
          <h1 class="text-3xl md:text-5xl font-bold leading-tight">
            I build
            <span
              class="text-transparent bg-clip-text bg-gradient-to-r from-primary to-purple-400"
            >
              modern web experiences
            </span>
            with motion & depth.
          </h1>

          <!-- description -->
          <p class="mt-6 text-white/70 leading-relaxed max-w-xl">
            I’m a frontend developer focused on crafting immersive, fast and
            scalable web experiences using Vue, Nuxt and modern UI systems.
          </p>

          <!-- features -->
          <div class="mt-10 space-y-3">
            <div class="feature">
              <span class="dot bg-primary"></span>
              Motion-first UI systems
            </div>

            <div class="feature">
              <span class="dot bg-purple-400"></span>
              High-performance Nuxt apps
            </div>

            <div class="feature">
              <span class="dot bg-cyan-400"></span>
              Clean scalable architecture
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
/* floating background */
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
  animation: float 10s ease-in-out infinite;
}
.float-slow {
  animation: float 14s ease-in-out infinite;
}

/* entrance animations */
@keyframes fadeUp {
  from {
    opacity: 0;
    transform: translateY(40px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

.image-reveal {
  animation: fadeUp 1s ease-out both;
}

.text-reveal {
  animation: fadeUp 1.2s ease-out both;
}

/* feature rows */
/* responsive fix polish */
@media (max-width: 768px) {
  .image-reveal img {
    height: 380px;
  }
}
</style>
