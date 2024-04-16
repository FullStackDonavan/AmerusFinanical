<template>
  <SectionContainer class="text-center">
    <div>
      <NuxtImg
        format="webp"
        src="/images/dental-insurance-banner.jpg"
        alt="Happy Kids"
        quality="80"
        class="full-width-height"
      />
    </div>
  </SectionContainer>
</template>

<script>
export default {
  name: "HomepageHeroSection",
  data() {
    return {
      IntroText: {
        SubHeading: "Our Commitment to Excellence",
        Heading: "About Good Time Travel",
        Description:
          "Good Time Travel is a nationwide leading bus charter company providing quality transportation and personal service for point-to-point excursions, long-distance, overnight trips, special events and more. No matter where you are traveling in the United States, our bus charter rentals offer safe, reliable transportation at affordable rates for both large and small groups. We pride ourselves on delivering extensive services to fulfill all your transportation needs with first-rate customer service and safety as our top priorities. Our experienced staff will support and guide you from the first call to the last mile so that your bus rental and trip goes exactly as planned.",
      },
      Featured: [
        {
          id: 1,
          title: "Commitment to Safety",
          description:
            "Providing secure transportation with top-notch safety measures for all our passengers.",
        },
        {
          id: 2,
          title: "Unparalleled Customer Service",
          description:
            "Ensuring a seamless journey from start to finish with personalized attention and support.",
        },
        {
          id: 3,
          title: "Reliable and Affordable Travel",
          description:
            "Offering dependable and cost-effective transportation solutions tailored to your needs.",
        },
      ],
      CTA: {
        to: "/get-started",
        text: "Get Started Now!",
      },
    };
  },
};
</script>

<style scoped>
.image-container {
  width: 100%;
  height: 100%;
  overflow: hidden;
}

.full-width-height {
  width: 100%;
  height: 100%;
  object-fit: cover; /* Ensure the image covers the entire container */
}
</style>
