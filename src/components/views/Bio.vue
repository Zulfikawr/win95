<template>
  <div>
      <h2 class="header">Muhammad Zulfikar</h2>
      <h4 class="subtitle" style="padding-bottom: 10px">
        Data Analyst | Quantitative Research | International Relations
      </h4>
      <h4 class="subtitle">Jakarta, Indonesia</h4>


    <div class="badge-grid">
      <img
        class="badge"
        alt="Python"
        src="https://img.shields.io/badge/-Python-darkblue"
      />

      <img
        class="badge"
        alt="SQL"
        src="https://img.shields.io/badge/-SQL-grey"
      />      

      <img
        class="badge"
        alt="NoSQL"
        src="https://img.shields.io/badge/-NoSQL-purple"
      />

      <img
        class="badge"
        alt="R"
        src="https://img.shields.io/badge/-R-blue"
      />

      <img
        class="badge"
        alt="Excel"
        src="https://img.shields.io/badge/-Excel-darkgreen"
      />

      <img
        class="badge"
        alt="PowerBI"
        src="https://img.shields.io/badge/-PowerBI-orange"
      />

      <img
        class="badge"
        alt="Tableau"
        src="https://img.shields.io/badge/-Tableau-red"
      />

      <img
        class="badge"
        alt="JavaScript"
        src="https://img.shields.io/badge/-JavaScript-yellow"
      />

    </div>

    <br> <hr> <br>

    <div class="table-of-contents">
      <h3 class="heading">Table of Contents</h3>
      <ul>
        <li><a href="#about-me" @click.prevent="scrollToSection('about-me')">About Me</a></li>
        <li><a href="#educations" @click.prevent="scrollToSection('educations')">Educations</a></li>
        <li><a href="#experiences" @click.prevent="scrollToSection('experiences')">Experiences</a></li>
        <li><a href="#skills" @click.prevent="scrollToSection('skills')">Skills</a></li>
        <li><a href="#resume" @click.prevent="scrollToSection('resume')">Résumé</a></li>
      </ul>
    </div>

    <br> <hr>

    <div class="inner-content" id="about-me">
      <h3 class="heading"><b>About Me</b></h3>
      <p class="paragraph">
        Hello there! I'm Zulfikar from Jakarta, a 20-year-old student with a passion 
        for both International Relations and Data Analytics. Currently, I am in my 4th semester 
        at Universitas Pembangunan Nasional Veteran Jakarta.
      </p>
      <p class="paragraph">
        Outside of my classes, I like to focus on practical ways to improve what I'm learning. 
        I believe there's more to learning than just textbooks. I particularly enjoy working on 
        data analytics projects. My goal is to bring together Data and International Relations 
        to make a positive impact in those fields. I want to create positive changes and improve 
        understanding between nations.
      </p> <br>
    </div>

    <hr>

    <div class="inner-content" id="educations">
      <h3 class="heading"><b>Educations</b></h3>
      <p class="paragraph">
        <b>Universitas Pembangunan Nasional Veteran Jakarta</b><br>
        International Relations <span class="year">2021 - Present</span><br>
        <li>GPA: 3.71 / 4.00</li>
      </p>
      <p class="paragraph">
        My studies at International Relations UPNVJ were both challenging and rewarding. 
        I learned a lot about world issues, how to think critically, and how to analyze information. 
        This prepared me well for a future career in international relations. Being part of "Himpunan 
        Mahasiswa Hubungan Internasional UPNVJ" was also a great experience. I made friends, learned 
        leadership and organizations skills, and participated in activities that helped me understand 
        International Relations even better.
      </p><br>

      <p class="paragraph">
        <b>Madrasah Aliyah Negeri 2 Jakarta</b> <br>
        Languages and Communications <span class="year">2018 - 2021</span><br>
        <li>GPA: 88.4 / 100</li>
      </p>
      <p class="paragraph">
        My high school experience at MAN 2 Jakarta was focused on foreign languages and communications. 
        This program helped me develop strong skills in both areas, which have been valuable in my life. 
        Being a part of MPK (Majelis Perwakilan Kelas) not only provided me with leadership experience and 
        teamwork skills but also helped me understand the diverse perspectives of my classmates. 
        I consistently performed well academically, even ranking at the top of my class. 
        Interestingly, while excelling in language and communication, my favorite subject, and the one 
        where I achieved my highest score, was actually math, which highlight my diverse academic interests.
      </p> <br>

    </div>

    <hr>

    <div class="inner-content" id="experiences">
      <h3 class="heading"><b> Experiences </b></h3>
      <p class="paragraph">
        <b> Quantium | Data Science & AI </b><br>
        Data Analyst <span class="year">Dec 2023 - Feb 2024</span><br>
      </p>
      <p class="paragraph">
        I recently participated in Quantium's Virtual Internship, and it was incredibly useful 
        to understand what it might be like to participate on a data analyst team at Quantium.
        I worked on a tasks to conduct analyses on a client's transaction dataset and
        identify customer purchasing behaviours to generate insights and provide
        commercial recommendations. I used Python and built my Data Visualisation in PowerBI. 
        <br> <br>

        My responsibilities in this internship included:
        <br> <br>

        <li>Analyzed transaction and customer data to identify trends and inconsistencies.</li>
        <li>Developed metrics and examine sales drivers to gain insights into overall sales performance.</li>
        <li>Created visualizations and prepare findings to formulate a clear recommendation for the client's strategy.</li>
        <li>Defined metrics to select control stores.</li>
        <li>Analyzed trial stores against controls.</li>
        <li>Used Python for data analysis and visualization and summarise findings and provide recommendations.</li>
        <li>Used the Pyramid Principles framework for structuring the report.</li>
        <li>Created a report that incorporates data visualizations, key insights, and recommendations.</li>
      </p> <br>

      <p class="paragraph">
        <b> IDX Partners x Rakamin Academy </b> <br>
        Data Scientist <span class="year">Dec 2023</span>
      </p>
      <p class="paragraph">
        I participated in the IDX Partners x Rakamin Academy Virtual Internship as a Data Scientist for one 
        month. During that time, I learned data science methodology and was challenged to master and implement 
        various skills and tools commonly used at IDX Partners, such as Big Data Fundamentals, Statistics 
        & Data Analytics, SQL Querying, R Programming, Python Programming, Machine Learning, and others.

        <br> <br>

        As the final task of my internship as a Data Scientist at IDX Partners, I was involved in a project 
        with a lending company. I collaborated with various departments on this project to provide 
        technological solutions for the company. My assignment was to build a model capable of predicting 
        credit risk using a dataset provided by the company, consisting of both accepted and rejected loan 
        data. Additionally, I needed to prepare visual media to present the solution to the client. 
        I ensured that the visual media I created was clear, easily readable, and communicative. 
        The end-to-end solution development was done in my programming language of choice while adhering 
        to the Data Science framework/methodology.

        <br> <br>
        
        My responsibilities during the IDX Partners x Rakamin Academy Virtual Internship as a Data Scientist included: <br> <br>
        
        <li>Applying data science methodology to analyze transaction and customer data, identifying trends and inconsistencies.</li>
        <li>Mastering and implementing various skills and tools, such as Big Data Fundamentals, Statistics & Data Analytics, SQL Querying, R Programming, Python Programming, Machine Learning, and more.</li>
        <li>Collaborating with different departments in a lending company project to provide technological solutions.</li>
        <li>Building a predictive credit risk model using a dataset containing both accepted and rejected loan data.</li>
        <li>Preparing visual media to effectively present the developed solution to the client.</li>
        <li>Ensuring clarity, readability, and communicativeness in the visual media created.</li>
        <li>Developing the end-to-end solution using my programming language of choice within the Data Science framework/methodology.</li>
      </p> <br>

      <p class="paragraph">
        <b> SMRC (Saiful Mujani Research and Consulting) </b> <br>
        Data Collector <span class="year"> Nov 2023 </span>
      </p>
      <p class="paragraph">
        Working as a data collector at SMRC, the national political survey organization, provided me 
        with valuable insights into the field research process. Part of my responsibilities included 
        obtaining the necessary permits from local authorities at various administrative levels, such 
        as subdistrict, urban village, Hamlet, and Neighborhood, to ensure smooth survey operations in designated 
        areas. Additionally, I conducted face-to-face interviews with ten individuals every week to 
        gather their perspectives on their political subjectivity. After collecting this information, 
        I carefully converted it into digital data, ensuring accuracy and ease of analysis. Through 
        this experience, I developed my communication skills while gaining firsthand knowledge of the 
        crucial role data collection plays in informing political research and decision-making processes.
      </p> <br>
    </div>

    <hr>

    <div class="inner-content" id="skills">
      <h3 class="heading"><b>Skills</b></h3>
      <p class="paragraph">
        As a student interested in global issues and data science, I have worked hard to build many different 
        skills. It all started with learning basic office tools like Microsoft Office 365 and Google Workspace. 
        These tools helped me work well with others and manage documents easily. After that, I got really 
        interested in data analysis. I learned how to use Excel, Python, R, and SQL (Microsoft SQL Server, 
        Google BigQuery, MySQL) to find important information in large datasets and see patterns. <br> <br>
        To make these insights easier to understand, I learned how to create visualizations using tools like 
        Matplotlib, Power BI, Tableau, and Google Looker Studio. With each visualization, I learned how to 
        communicate complex information in a clear and interesting way, using eye-catching visuals to explain 
        the data. During this process, I also developed important soft skills, like analytical thinking, 
        communication, problem-solving, time management, teamwork, and presentation and interview skills. 
        These abilities helped me deal with challenges, work well with others, and explain my ideas clearly 
        and confidently. As I continue to learn and grow, I am excited to use my technical and personal skills 
        to contribute to interesting projects that help us understand the world better.
      </p> <br>
    </div>

    <hr>

    <div class="inner-content" id="resume">
      <h3 class="heading"><b>Résumé</b></h3>
      <button
        style="text-decoration: underline;"
        href="/files/resume.pdf"
        class="paragraph">
        Check out my résumé here.
      </button>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    scrollToSection(sectionId) {
      const element = document.getElementById(sectionId);
      if (element) {
        element.scrollIntoView({
          behavior: 'smooth',
          // block: 'start',
        });
      }
    },
  },
};
</script>

<style scoped>

.badge-grid {
  display: table;
  width: 100%;
  justify-content: center;
  text-align: center;
  align-items: center;
  margin-top: 20px;
}

.badge {
  width: auto;
  height: 20px;
  border-radius: 0px;
  font-size: 12px;
  padding-right: 10px;
  /* box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.12), 0 6px 20px 0 rgba(0, 0, 0, 0.1); */
}

.self {
  width: 100%;
  height: auto;
  /* border-radius: 5px; */
}

.subtitle {
  font-size: 12px;
  color: gray;
  text-align: center;
}

.heading {
  padding-bottom: 5px;
}

.header {
  padding-top: 20px;
  padding-bottom: 20px;
  text-align: center;
}

.inner-content {
  padding-top: 30px;
}

h2,
h4,
h3 {
  padding: 0;
  margin: 0;
}

p {
  /* text-align: justify; */
  font-size: 15px;
}
.year {
  float: right;
  font-size: 15px;
}

li {
  list-style: square;
  padding-top: 10px;
  font-size: 15px;
}

.table-of-contents li {
  margin-bottom: 5px;
}

.table-of-contents a {
  text-decoration: none;
  color: blue;
}

.table-of-contents a:hover {
  text-decoration: underline;
}

</style>
