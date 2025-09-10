<template>
  <div class="flex flex-wrap items-start justify-center gap-4 sm:gap-6 py-4 relative z-20 max-w-full overflow-x-hidden">
    <!-- col1: hidden on mobile, visible from lg -->
    <div class="hidden lg:flex flex-col gap-5 sm:gap-6" v-parallax data-rellax-speed="8">
      <div class="relative aspect-[2/3] w-36 lg:w-52 flex-none overflow-hidden rounded-xl bg-zinc-100 dark:bg-zinc-800">
        <NuxtImg
          placeholder
          sizes="sm:100vw md:50vw lg:220px"
          class="absolute inset-0 h-full w-full object-cover"
          src="/img/home/grid-01.jpg"
          alt="Alt text"
          format="webp"
          loading="lazy"
        />
      </div>
    </div>

    <!-- col2 -->
    <div class="flex flex-col gap-5 sm:gap-6 w-1/2 xs:w-1/3 md:w-1/5" v-parallax data-rellax-speed="5">
      <div class="relative aspect-[4/3] w-full flex-none overflow-hidden rounded-xl bg-zinc-100 dark:bg-zinc-800">
        <NuxtImg
          placeholder
          sizes="sm:100vw md:50vw lg:220px"
          class="absolute inset-0 h-full w-full object-cover"
          src="/img/home/grid-02.jpg"
          alt="Alt text"
          format="webp"
          loading="lazy"
        />
      </div>
      <div class="relative aspect-[3/4] w-full flex-none overflow-hidden rounded-xl bg-zinc-100 dark:bg-zinc-800">
        <NuxtImg
          placeholder
          sizes="sm:100vw md:50vw lg:220px"
          class="absolute inset-0 h-full w-full object-cover"
          src="/img/home/grid-03.jpg"
          alt="Alt text"
          format="webp"
          loading="lazy"
        />
      </div>
    </div>

    <!-- col3 -->
    <div class="flex flex-col gap-5 sm:gap-6 w-1/2 xs:w-1/3 md:w-1/5" v-parallax data-rellax-speed="0">
      <div class="relative aspect-[2/3] w-full flex-none overflow-hidden rounded-2xl bg-zinc-100 dark:bg-zinc-800">
        <NuxtImg
          placeholder
          sizes="sm:100vw md:50vw lg:380px"
          class="absolute inset-0 h-full w-full object-cover"
          src="/img/home/grid-07.jpg"
          alt="Alt text"
          format="webp"
          loading="lazy"
        />
      </div>
    </div>

    <!-- col4 -->
    <div class="flex flex-col gap-5 sm:gap-6 w-1/2 xs:w-1/3 md:w-1/5" v-parallax data-rellax-speed="1">
      <div class="relative aspect-[3/4] w-full flex-none overflow-hidden rounded-xl bg-zinc-100 dark:bg-zinc-800">
        <NuxtImg
          placeholder
          sizes="sm:100vw md:50vw lg:220px"
          class="absolute inset-0 h-full w-full object-cover"
          src="/img/home/grid-04.jpg"
          alt="Alt text"
          format="webp"
          loading="lazy"
        />
      </div>
      <div class="relative aspect-[4/3] w-full flex-none overflow-hidden rounded-xl bg-zinc-100 dark:bg-zinc-800">
        <NuxtImg
          placeholder
          sizes="sm:100vw md:50vw lg:220px"
          class="absolute inset-0 h-full w-full object-cover"
          src="/img/home/grid-05.jpg"
          alt="Alt text"
          format="webp"
          loading="lazy"
        />
      </div>
    </div>

    <!-- col5: hidden on mobile, visible from lg -->
    <div class="hidden lg:flex flex-col gap-5 sm:gap-6" v-parallax data-rellax-speed="3">
      <div class="relative aspect-[2/3] w-44 lg:w-52 flex-none overflow-hidden rounded-xl bg-zinc-100 dark:bg-zinc-800">
        <NuxtImg
          placeholder
          sizes="sm:100vw md:50vw lg:220px"
          class="absolute inset-0 h-full w-full object-cover"
          src="/img/home/grid-06.jpg"
          alt="Alt text"
          format="webp"
          loading="lazy"
        />
      </div>
    </div>
  </div>
</template>