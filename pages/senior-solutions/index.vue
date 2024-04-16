<template>
  <PatternSection>
    <BasicSection>
      <SeniorInsuranceSolutionHeroSection />
      <Breadcrumbs
        currentPageTitle="Senior Solutions"
        parentTitle="Insurance Services"
        parentUrl="/insurance-services/"
      />

      <BasicSection>
        <div class="h-full">
          <!-- Card -->
          <div
            class="max-w-4xl mb-4 mx-auto bg-indigo-300 dark:bg-indigo-900 shadow-lg rounded-lg"
            v-for="Service in Services"
            :key="Service.title"
          >
            <div class="px-6 py-5">
              <div class="flex items-start">
                <img :src="Service.image" class="mr-4" width="250" />
                <!-- Card content -->
                <div class="flex-grow truncate">
                  <!-- Card header -->
                  <div class="w-full sm:flex justify-between items-center mb-3">
                    <!-- Title -->
                    <h2
                      class="text-2xl leading-snug font-extrabold text-gray-50 truncate mb-1 sm:mb-0"
                    >
                      {{ Service.title }}
                    </h2>
                  </div>
                  <!-- Card body -->
                  <div class="flex items-end justify-between whitespace-normal">
                    <!-- Paragraph -->
                    <div class="max-w-md text-indigo-100">
                      <p class="mb-2">
                        {{ Service.excerpt }}
                      </p>
                    </div>
                    <!-- More link -->
                    <nuxt-link
                      class="flex-shrink-0 flex items-center justify-center text-indigo-600 w-10 h-10 rounded-full bg-gradient-to-b from-indigo-50 to-indigo-100 hover:from-white hover:to-indigo-50 focus:outline-none focus-visible:from-white focus-visible:to-white transition duration-150 ml-2"
                      :to="Service.url"
                    >
                      <span class="block font-bold"
                        ><span class="sr-only">Read more</span> -></span
                      >
                    </nuxt-link>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </BasicSection>
      <GetAnswersToYourQuestions />
    </BasicSection>
  </PatternSection>
</template>

<script>
export default {
  name: "Home Page",
  data() {
    return {
      Services: [
        {
          title: "Medicare",
          excerpt:
            "Medicare provides essential healthcare coverage for individuals aged 65 and older, as well as certain younger people with disabilities. It consists of several parts, including hospital insurance (Part A), medical insurance (Part B), and prescription drug coverage (Part D). Understanding Medicare options is crucial for effective healthcare planning.",
          image: "/images/Medicare.jpg",
          url: "/senior-solutions/medicare/",
        },
        {
          title: "Senior Dental",
          excerpt:
            "Senior dental care is vital for maintaining overall health and well-being. Many seniors face challenges accessing affordable dental services, leading to untreated dental issues. Understanding available insurance plans and seeking preventive care can ensure seniors maintain good oral health and quality of life in their golden years.",
          image: "/images/senior-dental.jpg",
          url: "/senior-solutions/senior-dental/",
        },
        {
          title: "Senior Life",
          excerpt:
            "Senior life insurance provides financial security for loved ones after one's passing. It helps cover funeral costs, outstanding debts, and provides a legacy for beneficiaries. Understanding policy options, such as term or whole life insurance, is crucial for seniors to ensure their final expenses are adequately covered.",
          image: "/images/senior-life.jpg",
          url: "/senior-solutions/senior-life/",
        },
      ],
    };
  },
};
</script>
<style>
ul li span {
  /*
     * We want the bullets outside of the list,
     * so the text is aligned. Now the actual bullet
     * is outside of the list’s container
     */
  list-style-position: outside !important;

  /*
     * Because the bullet is outside of the list’s
     * container, indent the list entirely
     */
  /* margin-left: 1em; */
}
.svg svg {
  width: 100px;
}
.logoSection {
  height: 300px;
}
</style>