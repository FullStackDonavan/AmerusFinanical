<template>
  <PatternSection>
    <BasicSection>
      <IndividualAndFamilyInsuranceServicesHeroSection />
      <Breadcrumbs
        currentPageTitle="Individual & Family"
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
          title: "Health Insurance",
          excerpt:
            "Whether you're looking to enhance your favorite room in your home with a beautiful splash of color or you're looking to update the walls in your home to give them a fresh, modern look, Amerus Pro Painting can help! We can bring palates with endless options and will help you select that perfect hue. Once the color and level of sheen are selected, we'll get to work preparing your walls and ceilings to receive the paint. Amerus Pro Painting provides a wide range of interior painting services.",
          image: "/images/healthcare-excerpt.jpg",
          url: "/individual-health-insurance/Health-Insurance/",
        },
        {
          title: "Life Insurance",
          excerpt:
            "An eye-catching exterior makes a statement! When it comes to house painting and exterior painting, no one delivers like Amerus Pro Painting. We won't cut corners on the prep work because we know that sets the foundation for a professional, lasting exterior paint job. And when the job is complete, Amerus Pro Painting wants you to have just as much pride and joy in the final ",
          image: "/images/marketplace.jpg",
          url: "/individual-health-insurance/Life-Insurance/",
        },

        {
          title: "Indexed Universal Life Insurance",
          excerpt:
            "Whether you're looking to enhance your favorite room in your home with a beautiful splash of color or you're looking to update the walls in your home to give them a fresh, modern look, Amerus Pro Painting can help! We can bring palates with endless options and will help you select that perfect hue. ",
          image: "/images/annuities-excerpt.jpg",
          url: "/individual-health-insurance/Indexed-Universal-Life-Insurance/",
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