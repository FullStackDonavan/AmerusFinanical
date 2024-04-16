<template>
  <BasicSection class="container mx-auto mt-20">
    <div class="p-4 sm:p-8">
      <HeadlineTwo>{{ IntroText.Headline }}</HeadlineTwo>
      <ParagraphDescription>
        {{ IntroText.description }}
      </ParagraphDescription>
    </div>
  </BasicSection>
</template>

<script>
export default {
  name: "Ideal Customers Section",
  props: {
    title: String,
    description: String,
    mediaFirst: Boolean,
    subTitle: String,
  },
  data() {
    return {
      colorMode: useColorMode(),
      IntroText: {
        Headline:
          "Empowering Futures: Amerus Financial Group - Your Trusted Insurance Partner for Over Two Decades",
        description:
          "Established for over two decades, Amerus Financial Group is a comprehensive insurance agency headquartered in the scenic city of Lakeland, Florida. With a track record that spans more than 20 years, we have specialized in delivering personalized insurance solutions to both families and businesses alike. Over the years, our reach has expanded to a nationwide client base, boasting over 4,000 satisfied customers from various walks of life. This broad and diverse clientele has positioned Amerus Financial as a trusted authority in the insurance sector, especially when it comes to navigating the intricate challenges posed by the constantly evolving landscape of insurance regulations and offerings. Our team of highly skilled agents is our most valuable asset. They are not just trained; they are empowered with the knowledge and tools needed to tackle even the most complex insurance queries and problems. Through rigorous training programs and real-world experience, our agents have honed their skills to simplify what can often be a perplexing and daunting process of purchasing insurance. Whether you have questions that are difficult to answer or you’re just starting to explore your insurance options, our experts are equipped to guide you. What sets us apart is our commitment to personalization. We don’t believe in one-size-fits-all solutions when it comes to insurance. We diligently review your existing insurance portfolio and financial situation to provide you with tailored recommendations that are uniquely aligned with your specific needs and objectives. This meticulous approach ensures that you don’t just buy insurance; you invest in a safety net that genuinely suits you. At Amerus Financial Group, our mission is to make the complexities of the insurance world understandable, providing you with the best possible options to secure your future. We pride ourselves on being not just a service but a dependable resource for all your insurance needs.",
      },
    };
  },
  computed: {
    // const isDark = this.$colorMode.value === "dark";
    isDark() {
      if (this.colorMode.preference === "dark") {
        return true;
      } else {
        return false;
      }
    },
  },
};
</script>

<style scoped>
</style>