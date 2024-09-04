<script lang="ts" setup>
</script>

<template>
  <section class="relative bg-[#121519] lg:pt-6 xl:pt-12">
    <div class="absolute top-0 left-0 w-full h-full">
      <div
        class="jarallax-img jarallax-container"
        style="position: absolute; top: 0px; left: 0px; width: 100%; height: 100%; overflow: hidden; z-index: -100; clip-path: polygon(0px 0px, 100% 0px, 100% 100%, 0px 100%);"
      />
    </div>
    <div class="container mx-auto relative z-10 pt-2 sm:pt-6 md:pt-12">
      <div class="flex justify-center pt-12">
        <div class="lg:w-3/4 xl:w-2/3 text-center pt-12 mt-1">
          <a
            href="#"
            class="inline-flex items-center text-sm font-semibold no-underline bg-yellow-500/10 text-yellow-500 rounded-full py-2 px-3"
          >
            <span class="font-semibold leading-snug">Leilõões v0.0.1</span>
            <i class="ai-arrow-right text-lg ml-2 -mr-1" />
          </a>
          <h1 class="text-4xl md:text-5xl lg:text-6xl text-white pt-3 mt-3 mb-4">
            Poderosa AI para otimizar seus leilões de imóveis
          </h1>
          <p class="text-white opacity-70 text-xl">
            Nossa plataforma robusta é projetada para lidar com grandes volumes de dados e processamento, tornando-a
            perfeita para leilões de imóveis de todos os tamanhos.
          </p>
        </div>
      </div>
    </div>

    <div
      class="d-none d-lg-block"
      style="height:480px;"
    />
    <div
      class="d-lg-none"
      style="height:400px;"
    />
    <div class="flex absolute bottom-0 left-0 w-full overflow-hidden -mb-1 text-[#fff]">
      <div
        class="relative left-1/2 -translate-x-1/2 shrink-0"
        style="width:3774px;"
      >
        <svg
          width="3774"
          height="201"
          viewBox="0 0 3774 201"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            d="M0 200.003C0 200.003 1137.52 0.188224 1873.5 0.000134392C2614.84 -0.189325 3774 200.003 3774 200.003H0Z"
            fill="currentColor"
          />
        </svg>
      </div>
    </div>
  </section>
</template>

<style lang="css" scoped>
.jarallax {
  position: relative;
  z-index: 0;
}
.jarallax-img {
  background-image: url("/img/hero-bg-pattern-BkpvxLpL.png");
  object-fit: cover;
  object-position: 50% 50%;
  max-width: none;
  position: fixed;
  top: 0px;
  left: 0px;
  width: 1541px;
  height: 777.475px;
  overflow: hidden;
  pointer-events: none;
  transform-style: preserve-3d;
  backface-visibility: hidden;
  margin-top: -71.2375px;
  transform: translate3d(0px, 31.2375px, 0px);
}
</style>
