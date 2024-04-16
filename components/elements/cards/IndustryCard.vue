<template>
  <div>
    <div class="container mx-auto">
      <div class="flex items-stretch -mx-4">
        <div class="flex-1 p-4">
          <div
            class="block overflow-hidden rounded-t-lg rounded-b-lg h-full shadow-lg"
          >
            <div class="p-4 bg-blue-400 dark:bg-amber-400 min-h-24">
              <h2
                class="mt-2 mb-2 font-bold text-2xl font-Heading text-center text-white"
              >
                {{ title }}
              </h2>
            </div>
            <!-- <p class="text-md text-justify">{{ description }}</p> -->
            <div>
              <NuxtImg
                class="min-w-64"
                format="webp"
                :src="image"
                sizes="sm:217px md:323px lg:376px xl:504px xxl:632px 2xl:700px"
                alt="Bus Driver"
                quality="80"
                loading="lazy"
              />
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "IndustryCard",
  props: {
    title: String,
    image: String,
    description: String,
    url: String,
  },
};
</script>

<style>
</style>
