
<template>
  <div>
    <AppHeader />

    <main class="students-page">

      <!-- Page Introduction -->
      <section class="page-intro">
        <div class="intro-container">
          <span class="eyebrow">
            THE PEOPLE OF ITE 18
          </span>

          <h1>Meet Our Students</h1>

          <p>
            Get to know a few of our students and learn more
            about the individuals who make up our ITE 18 community.
          </p>
        </div>
      </section>

      <!-- Student Profiles -->
      <section class="profiles-section">
        <div class="profiles-container">

          <div class="section-heading">
            <span class="eyebrow">
              GET TO KNOW OUR STUDENTS
            </span>

            <h2>Featured Students</h2>

            <p>
              A closer look at four members of ITE 18.
            </p>
          </div>

          <div class="student-list">

            <StudentCard
              name="Ashley Shanne Caiña"
              course="BS Information Technology"
              image="/images/Ashley.jpeg"
              description="A student who continues to learn, explore new ideas, and gain experiences throughout her journey in Information Technology."
              github="https://github.com/ashleycaina21-beep"
            />

            <StudentCard
              name="Kiesha Jae Calderon"
              course="BS Information Technology"
              image="/images/Kiesha Jae.jpeg"
              description="Always learning something new, she takes each experience as an opportunity to grow and improve her skills."
              github="https://github.com/kieshajaecalderon"
            />

            <StudentCard
              name="Elaine Mae Balbada"
              course="BS Information Technology"
              image="/images/Daug_Elaine.png"
              description="A growing IT student who embraces new challenges and continues to discover more about the world of technology."
              github="https://github.com/elainemaebalbada"
            />

            <StudentCard
              name="Richelle Ann W. Calabroso"
              course="BS Information Technology"
              image="/images/Chelle Ann.jpg"
              description="An aspiring IT professional who enjoys learning, building connections, and making meaningful memories along the way."
              github="https://github.com/calabrosorichelleann-workac"
            />

          </div>
        </div>
      </section>

    </main>

    <AppFooter />
  </div>
</template>

<style scoped>
.students-page {
  width: 100%;
  background-color: #F5F5F0;
}

/* =========================
   PAGE INTRODUCTION
========================= */

.page-intro {
  background-color: #F5F5F0;
  padding: 75px 40px 65px;
}

.intro-container {
  max-width: 1100px;
  margin: 0 auto;
}

.eyebrow {
  display: block;
  color: #5D866C;
  font-size: 13px;
  font-weight: bold;
  letter-spacing: 2px;
}

.intro-container h1 {
  color: #453F38;
  font-family: Georgia, serif;
  font-size: 46px;
  line-height: 1.2;
  margin: 15px 0 20px;
}

.intro-container p {
  color: #665F56;
  font-size: 16px;
  line-height: 1.8;
  max-width: 600px;
  margin: 0;
}

/* =========================
   STUDENT PROFILES
========================= */

.profiles-section {
  background-color: #E6D8C3;
  padding: 70px 40px 85px;
}

.profiles-container {
  max-width: 1100px;
  margin: 0 auto;
}

.section-heading {
  margin-bottom: 35px;
}

.section-heading h2 {
  color: #453F38;
  font-family: Georgia, serif;
  font-size: 36px;
  line-height: 1.2;
  margin: 14px 0;
}

.section-heading p {
  color: #665F56;
  font-size: 15px;
  line-height: 1.7;
  margin: 0;
}

/* Student Cards */

.student-list {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 30px;
}

/* =========================
   RESPONSIVE DESIGN
========================= */

@media (max-width: 768px) {

  .page-intro {
    padding: 55px 25px;
  }

  .intro-container h1 {
    font-size: 36px;
  }

  .intro-container p {
    font-size: 15px;
  }

  .profiles-section {
    padding: 55px 25px 65px;
  }

  .section-heading h2 {
    font-size: 30px;
  }

  .student-list {
    grid-template-columns: 1fr;
    gap: 22px;
  }

}

@media (min-width: 600px) and (max-width: 768px) {

  .student-list {
    grid-template-columns: repeat(2, minmax(0, 1fr));
  }

}
</style>
