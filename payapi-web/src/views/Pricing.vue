<template>
  <div class="pricing">
    <img
      class="img-circle"
      src="../assets/shared/desktop/bg-pattern-circle.svg"
      alt=""
    />
    <div class="div-container">
      <p class="title-container">Pricing</p>

      <div class="div-price-container">
        <div class="price-plan">
          <p class="title-price">Free Plan</p>
          <p>
            Build and test using our core set of products with up to 100 API
            requests
          </p>
          <p class="price">$0.00</p>
          <hr width="100%" />
          <div>
            <featurePricing :isOffered="true" :featureName="'Transaction'" />
            <featurePricing :isOffered="true" :featureName="'Auth'" />
            <featurePricing :isOffered="true" :featureName="'Identity'" />
            <featurePricing :isOffered="false" :featureName="'Investments'" />
            <featurePricing :isOffered="false" :featureName="'Assets'" />
            <featurePricing :isOffered="false" :featureName="'Liabilities'" />
            <featurePricing :isOffered="false" :featureName="'Income'" />
          </div>
          <hr width="100%" />

          <div class="div-button">
            <form id="form-price" action="./contact">
              <secondaryDarkBtn
                :form="'form-price'"
                :btnText="'Request Access'"
              />
            </form>
          </div>
        </div>

        <div class="price-plan">
          <p class="title-price">Basic Plan</p>
          <p>
            Launch your project with unlimited requests and no contractual
            minimums
          </p>
          <p class="price">$249.00</p>
          <hr width="100%" />
          <div>
            <featurePricing :isOffered="true" :featureName="'Transaction'" />
            <featurePricing :isOffered="true" :featureName="'Auth'" />
            <featurePricing :isOffered="true" :featureName="'Identity'" />
            <featurePricing :isOffered="true" :featureName="'Investments'" />
            <featurePricing :isOffered="true" :featureName="'Assets'" />
            <featurePricing :isOffered="false" :featureName="'Liabilities'" />
            <featurePricing :isOffered="false" :featureName="'Income'" />
          </div>
          <hr width="100%" />

          <div class="div-button">
            <form id="form-price" action="./contact">
              <secondaryDarkBtn
                :form="'form-price'"
                :btnText="'Request Access'"
              />
            </form>
          </div>
        </div>

        <div class="price-plan">
          <p class="title-price">Premium Plan</p>
          <p>
            Get tailored solutions, volume pricing, and dedicated support for
            your team
          </p>
          <p class="price">$499.00</p>
          <hr width="100%" />
          <div>
            <featurePricing :isOffered="true" :featureName="'Transaction'" />
            <featurePricing :isOffered="true" :featureName="'Auth'" />
            <featurePricing :isOffered="true" :featureName="'Identity'" />
            <featurePricing :isOffered="true" :featureName="'Investments'" />
            <featurePricing :isOffered="true" :featureName="'Assets'" />
            <featurePricing :isOffered="true" :featureName="'Liabilities'" />
            <featurePricing :isOffered="true" :featureName="'Income'" />
          </div>
          <hr width="100%" />

          <div class="div-button">
            <form id="form-price" action="./contact">
              <secondaryDarkBtn
                :form="'form-price'"
                :btnText="'Request Access'"
              />
            </form>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.pricing {
  width: 100%;
  height: 100%;
}

p {
  text-align: start;
  margin: 10px;
  line-height: 175%;
}

.img-circle {
  position: absolute;
  top: -600px;
  right: -200px;
}

.div-container {
  padding-left: 10%;
  padding-right: 10%;
}

.title-container {
  font-family: DM Serif Display;
  font-style: normal;
  font-weight: bold;
  font-size: 56px;
  color: #36536b;
  margin-top: 5%;
  margin-bottom: 5%;
}

.div-price-container {
  display: flex;
  justify-content: space-between;
}

.price-plan {
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  width: 30%;
  height: 100%;
}

.title-price {
  font-family: DM Serif Display;
  font-style: normal;
  font-weight: bold;
  font-size: 32px;
  color: #ba4270;
}

.price {
  font-family: DM Serif Display;
  font-style: normal;
  font-weight: bold;
  font-size: 56px;
  color: #36536b;
}

.div-button {
  margin-top: 5%;
  display: flex;
}
</style>

<script>
import featurePricing from "../components/FeaturePricing.vue";
import secondaryDarkBtn from "../components/Buttons/SecondaryBtnDark.vue";
export default {
  components: {
    featurePricing,
    secondaryDarkBtn,
  },
};
</script>