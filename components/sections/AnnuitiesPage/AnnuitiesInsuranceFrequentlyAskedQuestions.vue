<template>
  <BasicSection class="container mx-auto mt-20">
    <div class="text-center">
      <HeadlineTwo>Frequently Asked Questions</HeadlineTwo>
    </div>
    <div class="accordion">
      <div>
        <div class="accordion-item" v-for="(item, index) in items" :key="index">
          <ParagraphDescription
            class="accordion-header font-extrabold"
            @click="toggleItem(index)"
          >
            {{ item.title }}
          </ParagraphDescription>
          <Transition name="slide">
            <div
              class="accordion-body bg-blue-100"
              :class="{ hidden: !isActive(index) }"
            >
              {{ item.content }}
            </div>
          </Transition>
        </div>
      </div>
    </div>
  </BasicSection>
</template>


<script>
export default {
  name: "HealthcareFrequentlyAskedQuestions",
  props: {
    items: {
      type: Array,
      required: true,
    },
    active: {
      type: Number,
      default: null,
    },
  },
  data() {
    return {
      activeItem: this.active,
    };
  },
  methods: {
    toggleItem(index) {
      if (this.activeItem === index) {
        this.activeItem = null; // Close the currently open item
      } else {
        this.activeItem = index; // Open the clicked item
      }
    },
    isActive(index) {
      return this.activeItem === index;
    },
  },
};
</script>


<style>
.slide-enter-active,
.slide-leave-active {
  transition: height 0.5s ease;
}
.slide-enter,
.slide-leave-to {
  height: 0;
  overflow: hidden;
}
.accordion {
  border: 1px solid #ccc;
  margin-bottom: 1rem;
}

.accordion-item {
  border-bottom: 1px solid #ccc;
}

.accordion-header {
  cursor: pointer;
  padding: 1rem;
}

.accordion-body {
  padding: 1rem;
}
</style>
