<template>
  <BasicSection class="container mx-auto mt-20">
    <div class="p-4 sm:p-8">
      <GridThreeColumns>
        <div
          class="mx-auto mb-4 bg-indigo-300 dark:bg-indigo-900 shadow-lg rounded-lg"
        >
          <div class="px-6 py-5">
            <div class="flex items-start">
              <!-- Card content -->
              <div class="flex-grow truncate">
                <!-- Card header -->
                <div class="w-full sm:flex justify-between items-center mb-3">
                  <!-- Title -->
                  <h2
                    class="text-2xl leading-snug font-extrabold text-gray-50 truncate mb-1 sm:mb-0 mx-auto"
                  >
                    Safety
                  </h2>
                </div>
                <!-- Card body -->
                <div class="flex items-end justify-between whitespace-normal">
                  <!-- Paragraph -->
                  <div class="max-w-md text-indigo-100">
                    <p class="mb-2">
                      Fixed annuities are considered one of the safest vehicles
                      available for your investment dollars and offer peace of
                      mind knowing that your hard earned savings are protected
                      from market fluctuations. Since the interest is not
                      dependent on the performance of stocks or any market
                      performance you don't have to worry about losing money
                      when the market falls. To date there has never been one
                      dollar lost in a fixed annuity contract.
                    </p>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>

        <div
          class="mx-auto mb-4 bg-indigo-300 dark:bg-indigo-900 shadow-lg rounded-lg"
        >
          <div class="px-6 py-5">
            <div class="flex items-start">
              <!-- Card content -->
              <div class="flex-grow truncate">
                <!-- Card header -->
                <div class="w-full sm:flex justify-between items-center mb-3">
                  <!-- Title -->
                  <h2
                    class="text-2xl leading-snug font-extrabold text-gray-50 truncate mb-1 sm:mb-0 mx-auto"
                  >
                    Liquidity
                  </h2>
                </div>
                <!-- Card body -->
                <div class="flex items-end justify-between whitespace-normal">
                  <!-- Paragraph -->
                  <div class="max-w-md text-indigo-100">
                    <p class="mb-2">
                      Annuity withdrawals are the contract provision that offers
                      liquidity and allows the owner to regularly withdraw
                      money. There are typically five different ways to withdraw
                      funds from an annuity befor the contract ends.
                    </p>
                    <p class="mb-2">Penalty Free Withdrawels</p>
                    <BasicList>
                      <ListItems
                        >Accumulating Penalty-Free Withdrawals</ListItems
                      >
                      <ListItems>Return of Premium</ListItems>
                      <ListItems>Systematic Withdrawals</ListItems>
                      <ListItems>Health-Related Waivers</ListItems>
                    </BasicList>
                    <p class="mb-2">
                      In addition annuities offer many income options that
                      provides a guaranteed income for the rest of your life.
                    </p>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>

        <div
          class="mx-auto mb-4 bg-indigo-300 dark:bg-indigo-900 shadow-lg rounded-lg"
        >
          <div class="px-6 py-5">
            <div class="flex items-start">
              <!-- Card content -->
              <div class="flex-grow truncate">
                <!-- Card header -->
                <div class="w-full sm:flex justify-between items-center mb-3">
                  <!-- Title -->
                  <h2
                    class="text-2xl leading-snug font-extrabold text-gray-50 truncate mb-1 sm:mb-0 mx-auto"
                  >
                    Tax Benefits
                  </h2>
                </div>
                <!-- Card body -->
                <div class="flex items-end justify-between whitespace-normal">
                  <!-- Paragraph -->
                  <div class="max-w-md text-indigo-100">
                    <p class="mb-2">
                      Usually, the funds that are paid into the investment are
                      tax-deferred until you start accepting annuity payments.
                      The taxes you pay are only regular income taxes too, which
                      means that you pay taxes on the income just like you would
                      any other income you receive. However, you can purchase
                      annuities with after-tax money too. If you do that, you
                      don’t have to pay taxes when you receive it until you
                      receive your principal back. All earnings from annuities
                      are subject to ordinary income tax.
                    </p>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </GridThreeColumns>
    </div>
  </BasicSection>
</template>

<script>
export default {
  name: "Important Features To A Fixed Annuity Section",
  data() {
    return {
      colorMode: useColorMode(),
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