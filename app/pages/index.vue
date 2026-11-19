
<template>
  <div>
    <AppHeader />

    <main class="home-page">

      <!-- HERO SECTION -->
      <section class="hero-section">
        <div class="hero-container">

          <!-- Hero Text -->
          <div class="hero-content">
            <span class="hero-label">
              ITE 18 · CARAGA STATE UNIVERSITY
            </span>

            <h1>
              Welcome to our ITE 18 class!
            </h1>

            <p>
              A place to get to know our class, the people in it,
              and the experiences we share.
            </p>

            <AppButton
              label="Meet Our Students →"
              color="#5D866C"
              to="/students"
            />
          </div>

          <!-- Hero Image with Decorations -->
          <div class="hero-image-wrapper">

            <div class="photo-blob"></div>

            <img
              src="/images/hero-class.jpg"
              alt="ITE 18 classmates together"
              class="hero-image"
            >

            <span class="sparkle sparkle-one">✧</span>
            <span class="sparkle sparkle-two">✦</span>

            <span class="heart-decoration">♡</span>

            <div class="leaf-decoration">
              <span></span>
              <span></span>
              <span></span>
            </div>

          </div>

        </div>
      </section>

      <!-- ABOUT OUR CLASS SECTION -->
      <section class="about-section">
        <div class="about-container">

          <span class="about-label">
            GET TO KNOW US
          </span>

          <h2>About Our Class</h2>

          <div class="about-divider"></div>

          <p>
            ITE 18 is a group of third-year BS Information Technology
            students from Caraga State University. Throughout our
            college journey, we continue to learn, explore new
            technologies, work together, and gain experiences that
            help us grow as future IT professionals.
          </p>

        </div>

        <!-- Decorative Leaves -->
        <div class="about-leaves about-leaves-left">
          <span></span>
          <span></span>
          <span></span>
        </div>

        <div class="about-leaves about-leaves-right">
          <span></span>
          <span></span>
          <span></span>
        </div>
      </section>

      <!-- CLASS HIGHLIGHTS SECTION -->
      <section class="highlights-section">
        <div class="highlights-container">

          <div class="highlights-heading">
            <span>OUR CLASS AT A GLANCE</span>

            <h2>What Makes Our Class Special</h2>

            <p>
              More than just a classroom, ITE 18 is a place where
              we learn, grow, and create meaningful connections.
            </p>
          </div>

          <div class="highlights-grid">

            <InfoCard
              title="Learning Together"
              description="We explore new technologies, share knowledge, and develop our skills as future IT professionals."
            />

            <InfoCard
              title="Growing Together"
              description="We learn from challenges, gain new experiences, and support one another throughout our college journey."
            />

            <InfoCard
              title="Building Connections"
              description="We create friendships, share memories, and build meaningful connections with our classmates."
            />

          </div>

        </div>
      </section>

    </main>

    <AppFooter />
  </div>
</template>

<style scoped>

/* =========================
   HOME PAGE
========================= */

.home-page {
  width: 100%;
  overflow: hidden;
}

/* =========================
   HERO SECTION
========================= */

.hero-section {
  background-color: #F5F5F0;
  padding: 75px 40px;
}

.hero-container {
  max-width: 1200px;
  min-height: 430px;
  margin: 0 auto;

  display: grid;
  grid-template-columns: 1fr 1fr;
  align-items: center;
  gap: 55px;
}

/* Hero Text */

.hero-content {
  max-width: 560px;
}

.hero-label {
  display: block;
  color: #5D866C;
  font-size: 14px;
  font-weight: bold;
  letter-spacing: 1.5px;
  margin-bottom: 20px;
}

.hero-content h1 {
  color: #453F38;
  font-family: Georgia, serif;
  font-size: 52px;
  line-height: 1.12;
  margin: 0 0 22px;
}

.hero-content p {
  color: #665F56;
  font-size: 17px;
  line-height: 1.7;
  max-width: 480px;
  margin-bottom: 30px;
}

/* =========================
   HERO IMAGE
========================= */

.hero-image-wrapper {
  position: relative;
  width: 100%;
  max-width: 540px;
  height: 390px;
  margin: 0 auto;

  display: flex;
  align-items: center;
  justify-content: center;
}

.photo-blob {
  position: absolute;
  inset: 5px;

  background-color: #C7D1BE;

  border-radius:
    45% 55% 60% 40% /
    45% 40% 60% 55%;

  transform: rotate(-5deg);
}

.hero-image {
  position: relative;
  z-index: 1;

  max-width: 100%;
  width: 100%;
  height: 100%;

  object-fit: cover;
  object-position: center;

  border-radius:
    45% 55% 60% 40% /
    45% 40% 60% 55%;

  display: block;
}

/* Sparkle Decorations */

.sparkle {
  position: absolute;
  z-index: 2;
  color: #5D866C;
  font-size: 40px;
}

.sparkle-one {
  top: 5px;
  left: -20px;
}

.sparkle-two {
  top: 25px;
  right: -15px;
}

/* Heart Decoration */

.heart-decoration {
  position: absolute;
  z-index: 2;

  bottom: 0;
  right: -20px;

  color: #5D866C;
  font-size: 55px;

  transform: rotate(12deg);
}

/* Leaf Decoration */

.leaf-decoration {
  position: absolute;
  z-index: 2;

  bottom: 5px;
  left: -30px;

  width: 65px;
  height: 80px;
}

.leaf-decoration span {
  position: absolute;

  width: 23px;
  height: 38px;

  background-color: #91A58B;

  border-radius: 100% 0 100% 0;
}

.leaf-decoration span:nth-child(1) {
  left: 5px;
  bottom: 0;
  transform: rotate(-35deg);
}

.leaf-decoration span:nth-child(2) {
  left: 25px;
  bottom: 20px;
  transform: rotate(35deg);
}

.leaf-decoration span:nth-child(3) {
  left: 0;
  bottom: 43px;
  transform: rotate(-45deg);
}

/* =========================
   ABOUT OUR CLASS
========================= */

.about-section {
  position: relative;

  background-color: #E6D8C3;

  padding: 75px 40px 85px;
  overflow: hidden;
}

.about-container {
  position: relative;
  z-index: 2;

  max-width: 900px;
  margin: 0 auto;

  text-align: center;
}

.about-label {
  display: block;

  color: #5D866C;
  font-size: 13px;
  font-weight: bold;
  letter-spacing: 2px;
}

.about-container h2 {
  color: #453F38;
  font-family: Georgia, serif;
  font-size: 42px;

  margin: 14px 0;
}

.about-divider {
  width: 65px;
  height: 3px;

  background-color: #5D866C;

  margin: 20px auto;
  border-radius: 5px;
}

.about-container p {
  color: #453F38;
  font-size: 17px;
  line-height: 1.9;

  margin: 0 auto;
}

/* About Section Leaves */

.about-leaves {
  position: absolute;
  width: 100px;
  height: 140px;
  opacity: 0.8;
}

.about-leaves span {
  position: absolute;

  width: 35px;
  height: 65px;

  background-color: #91A58B;

  border-radius: 100% 0 100% 0;
}

.about-leaves-left {
  left: -15px;
  bottom: 20px;
  transform: rotate(-25deg);
}

.about-leaves-right {
  right: -15px;
  bottom: 20px;
  transform: scaleX(-1) rotate(-25deg);
}

.about-leaves span:nth-child(1) {
  left: 5px;
  bottom: 0;
  transform: rotate(-25deg);
}

.about-leaves span:nth-child(2) {
  left: 35px;
  bottom: 35px;
  transform: rotate(25deg);
}

.about-leaves span:nth-child(3) {
  left: 0;
  bottom: 75px;
  transform: rotate(-40deg);
}

/* =========================
   CLASS HIGHLIGHTS SECTION
========================= */

.highlights-section {
  background-color: #F5F5F0;
  padding: 75px 40px;
}

.highlights-container {
  max-width: 1100px;
  margin: 0 auto;
}

.highlights-heading {
  text-align: center;
  max-width: 650px;
  margin: 0 auto 40px;
}

.highlights-heading span {
  color: #5D866C;
  font-size: 13px;
  font-weight: bold;
  letter-spacing: 2px;
}

.highlights-heading h2 {
  color: #453F38;
  font-family: Georgia, serif;
  font-size: 36px;
  margin: 15px 0;
}

.highlights-heading p {
  color: #665F56;
  font-size: 15px;
  line-height: 1.8;
  margin: 0;
}

.highlights-grid {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 25px;
}

/* =========================
   RESPONSIVE DESIGN
========================= */

@media (max-width: 900px) {

  .hero-container {
    gap: 30px;
  }

  .hero-content h1 {
    font-size: 42px;
  }

  .hero-image-wrapper {
    height: 320px;
  }

}

@media (max-width: 768px) {

  /* Hero */

  .hero-section {
    padding: 55px 25px;
  }

  .hero-container {
    grid-template-columns: 1fr;
    gap: 45px;
  }

  .hero-content {
    max-width: 100%;
    text-align: center;
  }

  .hero-content h1 {
    font-size: 40px;
  }

  .hero-content p {
    margin-left: auto;
    margin-right: auto;
  }

  .hero-image-wrapper {
    max-width: 480px;
    height: 300px;
  }

  /* About */

  .about-section {
    padding: 60px 25px 70px;
  }

  .about-container h2 {
    font-size: 34px;
  }

  .about-container p {
    font-size: 15px;
    line-height: 1.8;
  }

  .about-leaves {
    opacity: 0.35;
  }

  /* Class Highlights */

  .highlights-section {
    padding: 55px 25px;
  }

  .highlights-heading h2 {
    font-size: 30px;
  }

  .highlights-grid {
    grid-template-columns: 1fr;
    gap: 20px;
  }

}

@media (max-width: 480px) {

  .hero-content h1 {
    font-size: 34px;
  }

  .hero-label {
    font-size: 11px;
  }

  .hero-image-wrapper {
    height: 250px;
  }

  .sparkle {
    font-size: 28px;
  }

  .heart-decoration {
    font-size: 40px;
  }

  .about-container h2 {
    font-size: 30px;
  }

}

</style>
