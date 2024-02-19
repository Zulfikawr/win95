<template>
  <div>

    <img
      src="@/assets/Projects/projects.jpg"
      alt="Publications"
      class="hero"
    />

    <div class="inner-content">
        <h3 class="heading"><b>Projects</b></h3>
        <h4 class="subtitle">
          A complete lists of my projects. You can also see it in <a href="https://github.com/muhammad-zulfikar">GitHub</a>
        </h4>
    </div>

    <hr>

    <div class="inner-content">
      <p class="paragraph">
        <a href="https://github.com/muhammad-zulfikar/quantium" target="_blank">
          <b>Retail Analytics - Data Analysis at Quantium</b>
        </a> <br> <br>

        <iframe src="https://drive.google.com/file/d/1JaaSKAHkucj1SOx4q9HzT562fE0sHLJv/preview" 
          type="application/pdf"></iframe>

        <br>
        <p class="subtitle">Data Analysis, Python, PowerBI, PowerPoint</p> <br>
        I recently participated in Quantium's virtual internship.
        I worked on a project to conduct analyses on a client's transaction dataset and
        identify customer purchasing behaviours to generate insights and provide
        commercial recommendations. I used Python and built my Data Visualisation in PowerBI. 
        <br> <br>
        Project link: <a href="https://github.com/muhammad-zulfikar/quantium" target="_blank">GitHub</a> <br>
        Project documentation: <a href="https://www.notion.so/muhammad-zulfikar/quantium-Projects-4a6460df31db47bcb876bf4c3bdfbc98" target="_blank">Notion</a>
      </p>
    </div>

    <hr>

    <div class="inner-content">
      <p class="paragraph">
        <a href="https://github.com/muhammad-zulfikar/idxpartners_finalproject" target="_blank">
          <b>Credit Risk Predictive Model - Data Scientist at ID/X Partners</b>
        </a> <br> <br>

        <img
          src="@/assets/Projects/quantium.png"
          alt="Projects"
          class="hero"
        />

        <br>
        <p class="subtitle">Data Analysis, Python, PowerBI</p> <br>
        During my internship at ID/X Partners, I had the chance to work on an exciting final project. 
        I was given datasets of approved and rejected loan applications. My goal was to create a model 
        that could predict if a loan application would be approved or rejected. I used my skills in 
        Python programming to build this predictive model.
        <br> <br>

        Project link: <a href="https://github.com/muhammad-zulfikar/idxpartners_finalproject" target="_blank">GitHub</a> <br>
        Project documentation: <a href="https://www.notion.so/muhammad-zulfikar/ID-X-Partners-x-Rakamin-Academy-Internship-Final-Projects-53d9400e07fe429d831b2ed494bd295e" target="_blank">Notion</a>
      </p>
    </div>

  </div>
</template>

<style scoped>
.hero {
  width: 100%;
  background-position: center center;
  background-size: 100%;
  background-repeat: no-repeat;
  border: 1px solid rgb(0, 0, 0, 0.1);
}

.images {
  width: 100%;
  height: 350px;
  /* object-fit: cover; */
}

.images-full {
  width: 100%;
  height: auto;
  object-fit: cover;
}

.subtitle {
  font-size: 14px;
  color: gray;
  text-align: center;
}

.heading {
  padding-bottom: 5px;
}

.inner-content {
  padding-top: 30px;
  padding-bottom: 30px;
}

h6,
h3 {
  margin: 0;
  padding: 0;
  text-align: center;
}

p {
  text-align: justify;
  font-size: 15px;
}

iframe{
  width: 100%;
  height: 275px;
}

</style>