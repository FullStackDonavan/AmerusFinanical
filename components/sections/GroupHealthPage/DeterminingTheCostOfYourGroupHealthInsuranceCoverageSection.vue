<template>
  <BasicSection class="container mx-auto mt-20">
    <div class="px-4 sm:px-8">
      <HeadlineTwo>{{ IntroText.Headline }}</HeadlineTwo>
      <BasicList>
        <ListItems
          ><strong>The size of your group:</strong> Insurance works by the law
          of the large numbers. The larger your group the better chance you will
          receive lower rates. That is why some small groups may be better off
          to join an organization like NBBA to take advantage of group buynig
          power.</ListItems
        >
        <ListItems
          ><strong>The health of your group:</strong> Even though your business
          cannot be turned down for pre-existing conditiong there is a chance
          that you may qualify for better rates if your employees are relatively
          healthy.</ListItems
        >
        <ListItems
          ><strong>The location of your group:</strong> Each state and region
          may have different ratings based on a of community rating
          factors.</ListItems
        >
        <ListItems
          ><strong>The age of your group:</strong> The average age of your group
          will have a major roll to play inn determing the overall cost of your
          insurance coverage.</ListItems
        >
      </BasicList>
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
      IntroText: {
        SubHeading:
          "Secure Your Future: Amerus Financial Group - Your Independent Insurance Agency for Health, Annuities, Life, and Employee Benefits",
        Headline:
          "There are some important factors in determining the cost of your group health insurance coverage.",
        description:
          "Amerus Financial Group operates as an independant insurance agency with a focus on Health Insurance, Annuities, Life Insurance, and Employee Benefits. Our goal is to forge lasting connections with our clients, a commitment facilitated by our outstanding customer service. In line with this, we proudly collaborate with premier carriers in the industry, specifically selecting those whose business ideals align seamlessly with ours.",
      },
    };
  },
};
</script>