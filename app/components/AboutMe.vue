<template>
  <section class="relative overflow-hidden bg-black py-28">
    <!-- background -->
    <div class="absolute inset-0 bg-black/90 backdrop-blur-3xl"></div>

    <div
      class="absolute -top-40 -left-40 w-[500px] h-[500px] bg-primary/30 blur-[140px] rounded-full float"
    ></div>
    <div
      class="absolute bottom-0 right-0 w-[500px] h-[500px] bg-purple-500/20 blur-[160px] rounded-full float-slow"
    ></div>

    <!-- content -->
    <div class="relative z-10 container mx-auto px-6 pl-20">
      <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 items-center">
        <!-- Image -->
        <div class="lg:col-span-1"></div>
        <div class="lg:col-span-5 s">
          <div
            class="group relative rounded-2xl overflow-hidden border border-white/10"
          >
            <img
              src="https://plus.unsplash.com/premium_photo-1682146717223-874ac7dcc607?q=80&w=1170&auto=format&fit=crop"
              alt="About Me"
              class="w-full h-[600px] object-cover transition-all duration-700 group-hover:scale-110 group-hover:grayscale-0 grayscale"
            />
          </div>
        </div>

        <!-- Content -->
        <div class="lg:col-span-5 pt-35">
          <span class="text-primary uppercase tracking-[0.35em] text-xs">
            About Me
          </span>

          <div class="w-20 h-px bg-primary mt-1 mb-2"></div>

          <h2 class="text-4xl lg:text-6xl font-bold leading-tight">
            Building immersive
            <span class="">digital experiences</span>
          </h2>

          <p class="mt-8 text-white/70 leading-8 max-w-3xl">
            I'm a frontend developer specializing in Vue, Nuxt, and modern UI
            development. I enjoy transforming ideas into responsive,
            interactive, and visually engaging websites that combine performance
            with elegant design. I'm a frontend developer specializing in Vue,
            Nuxt, and modern UI development. I enjoy transforming ideas into
            responsive, interactive, and visually engaging websites that combine
            performance with elegant design.
          </p>

          <div class="grid grid-cols-1 md:grid-cols-2 gap-5 mt-10">
            <div
              class="group border-l border-primary rounded-xl p-5 hover: transition-all duration-300"
            >
              <h3
                class="font-semibold group-hover:text-primary transition-colors"
              >
                Frontend Development
              </h3>
              <p class="mt-2 text-sm text-white/60">
                Vue, Nuxt, Tailwind CSS, TypeScript
              </p>
            </div>
            <div
              class="group border-l border-primary rounded-xl p-5 hover: transition-all duration-300"
            >
              <h3
                class="font-semibold group-hover:text-primary transition-colors"
              >
                Frontend Development
              </h3>
              <p class="mt-2 text-sm text-white/60">
                Vue, Nuxt, Tailwind CSS, TypeScript
              </p>
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
