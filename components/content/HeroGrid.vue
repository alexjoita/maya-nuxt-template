<script setup lang="ts">
import { ref, onMounted, onBeforeUnmount } from "vue";
import type { PropType } from "vue";
import type { Image } from "../../types/image";

defineProps({
  image1: {
    type: Object as PropType<Image>,
    required: false,
  },
  image2: {
    type: Object as PropType<Image>,
    required: false,
  },
  image3: {
    type: Object as PropType<Image>,
    required: false,
  },
  image4: {
    type: Object as PropType<Image>,
    required: false,
  },
  image5: {
    type: Object as PropType<Image>,
    required: false,
  },
  image6: {
    type: Object as PropType<Image>,
    required: false,
  },
  image7: {
    type: Object as PropType<Image>,
    required: false,
  },
});

const defaultImage = "img/placeholder.jpg";

// Scroll to top button logic
const showScrollTop = ref(false);
function handleScroll() {
  showScrollTop.value = window.scrollY > 200;
}
function scrollToTop() {
  window.scrollTo({ top: 0, behavior: "smooth" });
}
onMounted(() => {
  window.addEventListener("scroll", handleScroll);
});
onBeforeUnmount(() => {
  window.removeEventListener("scroll", handleScroll);
});
</script>
<template>
  <div class="not-prose mt-8 sm:mt-24 content-visibility-visible contain-intrinsic-size-[auto_600px]">
    <div class="flex flex-col sm:flex-row items-center justify-center gap-5 py-4 sm:gap-6 relative z-20 w-full">
      <!-- col1 -->
      <div class="w-full sm:w-auto hidden lg:flex flex-col gap-5 sm:gap-6" v-parallax data-rellax-speed="3">
        <div class="relative aspect-[2/3] w-full sm:w-36 lg:w-52 flex-none overflow-hidden rounded-xl bg-zinc-100 dark:bg-zinc-800">
          <NuxtImg
            placeholder
            sizes="100vw sm:100vw md:50vw lg:220px"
            class="absolute inset-0 h-full w-full object-cover"
            :src="image1?.src ? image1.src : defaultImage"
            :alt="image1?.alt ? image1.alt : 'No alt text'"
            :width="image1?.width ? image1.width : 1"
            :height="image1?.height ? image1.height : 1"
            format="webp"
            loading="lazy"
          />
        </div>
      </div>

      <!-- col2 -->
      <div class="w-full sm:w-auto flex flex-col gap-5 sm:gap-6" v-parallax data-rellax-speed="1">
        <div class="relative aspect-[4/3] w-full sm:w-44 md:w-52 flex-none overflow-hidden rounded-xl bg-zinc-100 dark:bg-zinc-800">
          <NuxtImg
            placeholder
            sizes="100vw sm:100vw md:50vw lg:220px"
            class="absolute inset-0 h-full w-full object-cover"
            :src="image2?.src ? image2.src : defaultImage"
            :alt="image2?.alt ? image2.alt : 'No alt text'"
            :width="image2?.width ? image2.width : 1"
            :height="image2?.height ? image2.height : 1"
            format="webp"
            loading="lazy"
          />
        </div>
        <div class="relative aspect-[3/4] w-full sm:w-44 md:w-52 flex-none overflow-hidden rounded-xl bg-zinc-100 dark:bg-zinc-800">
          <NuxtImg
            placeholder
            sizes="100vw sm:100vw md:50vw lg:220px"
            class="absolute inset-0 h-full w-full object-cover"
            :src="image3?.src ? image3.src : defaultImage"
            :alt="image3?.alt ? image3.alt : 'No alt text'"
            :width="image3?.width ? image3.width : 1"
            :height="image3?.height ? image3.height : 1"
            format="webp"
            loading="lazy"
          />
        </div>
      </div>

      <!-- col3 -->
      <div class="w-full sm:w-auto flex flex-col gap-5 sm:gap-6" v-parallax data-rellax-speed="0">
        <div class="relative aspect-[2/3] w-full sm:w-72 md:w-80 lg:w-96 flex-none overflow-hidden rounded-2xl bg-zinc-100 dark:bg-zinc-800">
          <NuxtImg
            placeholder
            sizes="100vw sm:100vw md:50vw lg:380px"
            class="absolute inset-0 h-full w-full object-cover"
            :src="image4?.src ? image4.src : defaultImage"
            :alt="image4?.alt ? image4.alt : 'No alt text'"
            :width="image4?.width ? image4.width : 1"
            :height="image4?.height ? image4.height : 1"
            format="webp"
            loading="lazy"
          />
        </div>
      </div>

      <!-- col4 -->
      <div class="w-full sm:w-auto flex flex-col gap-5 sm:gap-6" v-parallax data-rellax-speed="1">
        <div class="relative aspect-[3/4] w-full sm:w-44 md:w-52 flex-none overflow-hidden rounded-xl bg-zinc-100 dark:bg-zinc-800">
          <NuxtImg
            placeholder
            sizes="100vw sm:100vw md:50vw lg:220px"
            class="absolute inset-0 h-full w-full object-cover"
            :src="image5?.src ? image5.src : defaultImage"
            :alt="image5?.alt ? image5.alt : 'No alt text'"
            :width="image5?.width ? image5.width : 1"
            :height="image5?.height ? image5.height : 1"
            format="webp"
            loading="lazy"
          />
        </div>
        <div class="relative aspect-[4/3] w-full sm:w-44 md:w-52 flex-none overflow-hidden rounded-xl bg-zinc-100 dark:bg-zinc-800">
          <NuxtImg
            placeholder
            sizes="100vw sm:100vw md:50vw lg:220px"
            class="absolute inset-0 h-full w-full object-cover"
            :src="image6?.src ? image6.src : defaultImage"
            :alt="image6?.alt ? image6.alt : 'No alt text'"
            :width="image6?.width ? image6.width : 1"
            :height="image6?.height ? image6.height : 1"
            format="webp"
            loading="lazy"
          />
        </div>
      </div>

      <!-- col5 -->
      <div class="w-full sm:w-auto hidden lg:flex flex-col gap-5 sm:gap-6" v-parallax data-rellax-speed="3">
        <div class="relative aspect-[2/3] w-full sm:w-44 lg:w-52 flex-none overflow-hidden rounded-xl bg-zinc-100 dark:bg-zinc-800">
          <NuxtImg
            placeholder
            sizes="100vw sm:100vw md:50vw lg:220px"
            class="absolute inset-0 h-full w-full object-cover"
            :src="image7?.src ? image7.src : defaultImage"
            :alt="image7?.alt ? image7.alt : 'No alt text'"
            :width="image7?.width ? image7.width : 1"
            :height="image7?.height ? image7.height : 1"
            format="webp"
            loading="lazy"
          />
        </div>
      </div>
    </div>

    <!-- Scroll to Top Button -->
    <button
      v-if="showScrollTop"
      @click="scrollToTop"
      class="fixed bottom-6 right-6 z-50 bg-white/80 dark:bg-zinc-900/80 text-zinc-800 dark:text-zinc-100 border border-zinc-200 dark:border-zinc-700 backdrop-blur-md shadow-lg rounded-full p-3 transition hover:bg-zinc-100 dark:hover:bg-zinc-800 hover:text-primary focus:outline-none focus:ring-2 focus:ring-primary"
      aria-label="Scroll to top"
    >
      <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 15l7-7 7 7" />
      </svg>
    </button>
  </div>
</template>
