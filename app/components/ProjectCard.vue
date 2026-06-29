<template>
  <article
    class="group relative overflow-hidden h-[250px] rounded-2xl border border-white/10 bg-black transition-all duration-500 hover:border-primary"
  >
    <!-- Image -->
    <div class="overflow-hidden">
      <img
        src="https://images.unsplash.com/photo-1518770660439-4636190af475?q=80&w=1400&auto=format&fit=crop"
        alt=""
        class="h-full w-full object-cover transition duration-700 group-hover:scale-105"
      />
    </div>

    <!-- Gradient -->
    <div
      class="absolute inset-0 bg-gradient-to-t from-black via-black/80 to-transparent transition duration-500 group-hover:from-black group-hover:via-black/60"
    ></div>

    <!-- Border Animation -->
    <div
      class="absolute inset-0 rounded-2xl ring-1 ring-transparent transition duration-500 group-hover:ring-primary"
    ></div>

    <!-- Content -->
    <div class="absolute inset-x-0 bottom-0 p-8 text-white">
      <span class="text-xs uppercase tracking-[0.35em] text-primary">
        Case Study · 2026
      </span>

      <h3
        class="mt-3 text-3xl font-semibold transition-colors duration-300 group-hover:text-primary"
      >
        Luxury Fashion Campaign
      </h3>

      <!-- Hidden Content -->
      <div
        class="overflow-hidden max-h-0 opacity-0 transition-all duration-500 group-hover:max-h-40 group-hover:opacity-100"
      >
        <p class="mt-4 max-w-md text-sm leading-7 text-white/70">
          Creative direction, web animation and immersive storytelling built
          with Nuxt, GSAP and a headless CMS.
        </p>

        <div
          class="mt-6 inline-flex items-center gap-2 text-sm font-medium text-primary"
        >
          View Project

          <svg
            class="h-4 w-4 transition-transform duration-300 group-hover:translate-x-1"
            fill="none"
            stroke="currentColor"
            stroke-width="2"
            viewBox="0 0 24 24"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              d="M5 12h14m-6-6 6 6-6 6"
            />
          </svg>
        </div>
      </div>
    </div>
  </article>
</template>

<style scoped>
article {
  transition:
    transform 0.45s ease,
    border-color 0.45s ease,
    box-shadow 0.45s ease;
}

article:hover {
  transform: translateY(-8px);
  border-color: var(--primary);
  box-shadow:
    0 30px 60px rgba(0, 0, 0, 0.45),
    0 0 0 1px rgba(255, 255, 255, 0.05),
    0 0 40px rgb(var(--primary));
}
</style>
