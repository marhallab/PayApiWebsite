<template>
  <div class="about">
    <section class="section1">
      <img
        class="img-circle-section1"
        src="../assets/shared/desktop/bg-pattern-circle.svg"
        alt=""
      />
      <div class="div-container-title-text">
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

    <section class="section2">
      <img
        class="img-section2"
        src="../assets/about/desktop/image-team-members.jpg"
        alt=""
      />

      <img
        class="img-circle-section2"
        src="../assets/shared/desktop/bg-pattern-circle.svg"
        alt=""
      />

      <div class="infos-container">
        <div class="info-section2">
          <hr width="100%" />
          <p>Team Members</p>
          <p>300+</p>
          <hr class="dividerGone" width="100%" />
        </div>

        <div class="info-section2">
          <hr class="dividerGone" width="100%" />
          <p>Offices in the US</p>
          <p>3</p>
          <hr class="dividerGone" width="100%" />
        </div>

        <div class="info-section2">
          <hr class="dividerGone" width="100%" />
          <p>Transactions analyzed</p>
          <p>10M+</p>
          <hr width="100%" />
        </div>
      </div>
    </section>

    <section class="section3">
      <div class="div-container-title-text">
        <div class="title-text">
          <p>The Culture</p>
          <p>
            We strongly believe there's always an opportunity to learn from each
            other outside of day-to-day work, whether it's company-wide
            offsites, internal hackathons, or co-worker meetups. We always value
            cross-team collaboration and diversity of thought, no matter the job
            title.
          </p>
        </div>

        <div class="title-text">
          <p>The People</p>
          <p>
            We're all passionate about building a more efficient and inclusive
            financial infrastructure together. At PayAPI, we have diverse
            backgrounds and skills.
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

.div-container-title-text {
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

.img-circle-section1 {
  position: absolute;
  top: -600px;
  right: -200px;
}

/*Section 2*/
.section2 {
  padding-top: 10%;
}

.img-circle-section2 {
  position: absolute;
  top: 650px;
  right: 1000px;
}

.img-section2 {
  position: relative;
  z-index: 1;
  width: 100%;
  height: auto;
}

.infos-container {
  display: flex;
  justify-content: space-evenly;
  padding-top: 7%;
}

.info-section2 {
  width: 23%;
}

.info-section2 p:last-of-type {
  font-family: DM Serif Display;
  font-style: normal;
  font-weight: bold;
  font-size: 56px;
  line-height: 72px;
  color: #ba4270;
}

/*Section 3*/
.section3 {
  padding-left: 15%;
  padding-right: 15%;
  padding-top: 5%;
}

@media only screen and (max-width: 1024px) {
  .title-section1 {
    text-align: center;
    font-size: 40px;
    width: 100%;
  }

  .img-circle-section1 {
    position: absolute;
    top: -600px;
    right: -500px;
  }
}

@media only screen and (max-width: 500px) {
  p {
    text-align: center;
  }

  .title-text {
    flex-direction: column;
  }

  .title-text p:first-child {
    width: 100%;
  }

  .title-text p:last-child {
    margin-left: 5%;
    width: 100%;
  }
  .infos-container {
    flex-direction: column;
    align-items: center;
  }

  .info-section2 {
    width: 80%;
  }

  .dividerGone {
    display: none;
  }
}
</style>