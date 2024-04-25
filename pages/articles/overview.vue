

<template>
  <PatternSection class="flex justify-center w-100">
    <ContentList path="/articles" v-slot="{ list }">
      <div class="flex flex-col justify-center w-100">
        <div
          v-for="article in list"
          :key="article._path"
          class="max-w-xl rounded overflow-hidden shadow-xl transition duration-500 hover:scale-110 my-10 p-0 dark:bg-text-white min-h-[180px]"
        >
          <NuxtLink :to="article._path" v-if="article.img">
            <GridTwoColumns>
              <div class="mr-4">
                <img :src="article.img" alt="" />
              </div>
              <div>
                <div class="p-4">
                  <div class="font-bold text-xl mb-2 dark:text-white">
                    {{ article.title }}
                  </div>
                  <p class="text-gray-700 dark:text-white text-base">
                    {{ article.description }}
                  </p>
                </div>
              </div>
            </GridTwoColumns>
          </NuxtLink>
          <NuxtLink :to="article._path" v-else class="h-full">
            <div class="p-4">
              <div class="font-bold text-xl mb-2 dark:text-white">
                {{ article.title }}
              </div>
              <p class="text-gray-700 dark:text-white text-base">
                {{ article.description }}
              </p>
            </div>
          </NuxtLink>
        </div>
      </div>
    </ContentList>
  </PatternSection>
</template>