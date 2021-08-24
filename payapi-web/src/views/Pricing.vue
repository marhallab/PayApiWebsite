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
            <p>test</p>
            <p>test</p>
            <p>test</p>
            <p>test</p>
            <p>test</p>
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
</style>