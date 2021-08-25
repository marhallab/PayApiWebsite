<template>
  <div class="about">
    <section class="section1">
      <img
        class="img-circle"
        src="../assets/shared/desktop/bg-pattern-circle.svg"
        alt=""
      />
      <div class="div-container-section1">
        <p class="title-section1">
          We empower innovators by delivering access to the financial system
        </p>
        <div class="title-text">
          <p>Our Vision</p>
          <p>
            Our main goal is to build beautiful consumer experiences along with
            developer-friendly infrastructure. The result is an intelligent tool
            that gives everyone the ability to create amazing products that
            solve big problems. We are deeply focused on democratizing financial
            services through technology.
          </p>
        </div>

        <div class="title-text">
          <p>Our Business</p>
          <p>
            At the core of our platform is the technical infrastructure APIs
            that connect consumers. Our innovative product provides key insights
            for businesses and individuals, as well as robust reporting for
            traditional financial institutions and developers.
          </p>
        </div>
      </div>
    </section>
  </div>
</template>

<style scoped>
.about {
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

.title-text {
  display: flex;
  width: 100%;
  margin-top: 5%;
}

.title-text p:first-child {
  width: 80%;
  font-family: DM Serif Display;
  font-style: normal;
  font-weight: bold;
  font-size: 30px;
  line-height: 40px;
  color: #36536b;
}

.title-text p:last-child {
  margin-left: 5%;
  width: 200%;
}
/*Section 1*/
.section1 {
  padding-left: 15%;
  padding-right: 15%;
  padding-top: 5%;
}

.div-container-section1 {
  display: flex;
  flex-direction: column;
}

.title-section1 {
  font-family: DM Serif Display;
  font-style: normal;
  font-weight: bold;
  font-size: 56px;
  line-height: 56px;
  color: #36536b;
  width: 80%;
}
</style>