/* eslint-disable */
<template>
  <interact
    draggable
    :dragOption="dragOption"
    class="resize-drag"
    :style="style"
    @dragmove="dragmove"
    @resizemove="resizemove"
    :class="{ fullscreen: $store.getters.isFullscreenBio }"
  >
    <div
      class="window"
      id="container"
      :class="{
        fullscreen: $store.getters.isFullscreenBio,
        close: !$store.getters.isShownBio,
      }"
    >
      <div
        class="top-bar"
        id="top-bar"
        v-on:dblclick="$store.commit('toggleFullscreenBio')"
        :class="
          $store.getters.activeWindow == 'Bio'
            ? 'top-bar'
            : 'top-bar-deactivated'
        "
      >
        <div
          style="
            color: white;
            margin-left: 3px;
            display: flex;
            align-items: center;
          "
        >
          <img class="icon-image" src="../assets/win95Icons/bio.png" />Biography
        </div>
        <div class="triple-button">
          <div class="button-hide" v-on:click="minimizeBio">
            <span
              style="
                height: 2px;
                width: 6px;
                background: black;
                margin-top: 8px;
                margin-right: 2px;
              "
            ></span>
          </div>
          <div
            class="button-expand"
            v-on:click="$store.commit('toggleFullscreenBio')"
          >
            <span
              style="
                height: 8px;
                width: 9px;
                border-left: black 1px solid;
                border-right: black 1px solid;
                border-left: black 1px solid;
                border-bottom: black 1px solid;
                border-top: black 2px solid;
              "
            ></span>
          </div>
          <div
            style="margin-right: 3px; padding-left: 1px"
            class="button-close"
            v-on:click="closeBio"
          >
            ×
          </div>
        </div>
      </div>

      <div class="content">
        <div
          class="scroll-container"
          :class="{ expandedScrollContainer: $store.getters.isFullscreenBio }"
        >
        <center>
          <div class="header">Muhammad Zulfikar</div>
          <div class="subtitle">
            Data Analyst | Quantitative Research | International Relations
          </div>
          <div class="subtitle">Jakarta</div>

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
        </center>

          <div class="inner-content">
            <h3 class="heading"><b>About Me</b></h3>
            <p class="paragraph" style="text-align: justify;">
              Hello there! I am Zulfikar from Jakarta, and I'm 20 year old student
              who's extremely passionate in International Relations and Data Analytics.
              I am currently 4th semester student in Universitas Pembangunan Nasional
              Veteran Jakarta.
            </p>
            <p class="paragraph">
              I have worked with a mixture of design and frontend/backend
              technologies, be it for Web Development or iOS Development.
            </p>
          </div>

          <hr>

          <div class="inner-content">
            <h3 class="heading"><b>Educations</b></h3><br>
            <b>"Universitas Pembangunan Nasional Veteran Jakarta"</b>
            <p class="paragraph">
              - 2021 - Present <br>
              - Major: International Relations <br>
              - GPA: 3.71 / 4.00
            </p>
            <p class="paragraph">
              My studies at International Relations UPNVJ were both challenging and rewarding. 
              I learned a lot about world issues, how to think critically, and how to analyze information. 
              This prepared me well for a future career in international relations. Being part of "Himpunan 
              Mahasiswa Hubungan Internasional UPNVJ" was also a great experience. I made friends, learned 
              leadership and organizations skills, and participated in activities that helped me understand 
              Rnternational Relations even better.
            </p>
            <br> <br>

            <b>"Madrasah Aliyah Negeri 2 Jakarta"</b>
            <p class="paragraph">
              - 2018 - 2021 <br>
              - Major: Languages and Communications <br>
              - GPA: 88.4 / 100
            </p>
            <p class="paragraph">
              My high school experience at MAN 2 Jakarta was focused on foreign languages and communications. 
              This program helped me develop strong skills in both areas, which have been valuable in my life. 
              As a member of MPK (Majelis Perwakilan Kelas), not only provided me with leadership experience and 
              teamwork skills but also helped me understand the diverse perspectives of my classmates. 
              Additionally, I consistently performed well academically, even ranking at the top of my class. 
              Interestingly, while excelling in language and communication, my favorite subject, and the one 
              where I achieved my highest score, was actually math, which highlight my diverse academic interests. 
              This strong academic performance allowed me to secure admission to UPNVJ University through 
              the SNMPTN invitation program.
            </p>

          </div>

          <hr>

          <div class="inner-content">
            <h3 class="heading"><b>Experiences</b></h3><br>
            <b> Data Analyst - Quantium </b>
            <p class="paragraph">
              December 2023 - February 2024 <br> <br>
              I recently participated in Quantium's Virtual Internship, and it was incredibly useful 
              to understand what it might be like to participate on a data analyst team at Quantium.
              I worked on a project to conduct analyses on a client's transaction dataset and
              identify customer purchasing behaviours to generate insights and provide
              commercial recommendations. I used Python and built my Data Visualisation in PowerBI. 
              <br> <br>

              My responsibilities in this project included:
              <br> <br>

              - Analyzed transaction and customer data to identify trends and inconsistencies.<br>
              - Developed metrics and examine sales drivers to gain insights into overall sales performance. <br>
              - Created visualizations and prepare findings to formulate a clear recommendation for the client's strategy.<br>
              - Defined metrics to select control stores.<br>
              - Analyzed trial stores against controls.<br>
              - Used Python for data analysis and visualization and summarise findings and provide recommendations.<br>
              - Used the Pyramid Principles framework for structuring the report.<br>
              - Created a report that incorporates data visualizations, key insights, and recommendations.
            </p>

            <br> <br>

            <b> Data Scientist - IDX Partners </b>
            <p class="paragraph">
              December 2023 - February 2024 <br> <br>
              I recently participated in Quantium's Virtual Internship, and it was incredibly useful 
              to understand what it might be like to participate on a data analyst team at Quantium.
              I worked on a project to conduct analyses on a client's transaction dataset and
              identify customer purchasing behaviours to generate insights and provide
              commercial recommendations. I used Python and built my Data Visualisation in PowerBI. 
              <br> <br>

              My responsibilities in this internship included:
              <br> <br>

              - Analyzed transaction and customer data to identify trends and inconsistencies.<br>
              - Developed metrics and examine sales drivers to gain insights into overall sales performance. <br>
              - Created visualizations and prepare findings to formulate a clear recommendation for the client's strategy.<br>
              - Defined metrics to select control stores.<br>
              - Analyzed trial stores against controls.<br>
              - Used Python for data analysis and visualization and summarise findings and provide recommendations.<br>
              - Used the Pyramid Principles framework for structuring the report.<br>
              - Created a report that incorporates data visualizations, key insights, and recommendations.
            </p>

            <br> <br>
          </div>

          <div class="inner-content">
            <div class="heading"><b>Résumé</b></div>
            <a
              style="color: #ff5733"
              href="/files/don_chia_resume.pdf"
              class="paragraph"
              >Check out my résumé here.</a
            >
          </div>
        </div>
      </div>
    </div>
  </interact>
</template>

<style scoped>
.resize-drag {
  box-sizing: border-box;
  background: none;
  user-select: auto;
  -ms-touch-action: auto;
  touch-action: auto;
  min-height: 40px;
  min-width: 350px;
  position: sticky;
  cursor: auto !important;
}

.window {
  min-height: 500px;
  min-width: 350px;
  height: 500px;
  width: 600px;
  background: rgb(195, 195, 195);
  overflow: hidden;
  border-top: solid rgb(250, 250, 250) 2px;
  border-left: solid rgb(250, 250, 250) 2px;
  border-right: solid rgb(90, 90, 90) 1.5px;
  border-bottom: solid rgb(90, 90, 90) 1.5px;
  box-shadow: 1.5px 1.5px black;
  max-height: 100%;
  max-width: 100%;
  align-items: flex-end;
  outline: rgb(222, 222, 222) 1px solid;
}

.self {
  width: 100%;
  height: auto;
  /* border-radius: 5px; */
}

@media only screen and (max-width: 600px) {
  .window {
    min-width: 50vw;
    width: 90vw;
    max-width: 100vw;
  }
  .scroll-container {
    padding-left: 10vw !important;
    padding-right: 10vw !important;
  }
  .expandedScrollContainer {
    padding-left: 10vw !important;
    padding-right: 10vw !important;
  }
}

.button-expand,
.button-close,
.button-hide {
  background: rgb(195, 195, 195);
  border-top: solid rgb(250, 250, 250) 1px;
  border-left: solid rgb(250, 250, 250) 1px;
  border-right: solid rgb(90, 90, 90) 1px;
  border-bottom: solid rgb(90, 90, 90) 1px;
  box-shadow: 1px 1px black;
  height: 16px;
  width: 16px;
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 20px;
  font-weight: bold;
  margin-left: 2px;
}

.button-close:hover,
.button-expand:hover,
.button-hide:hover {
  cursor: pointer;
}

.button-close:active,
.button-expand:active,
.button-hide:active {
  border-radius: 0px;
  background: rgb(192, 192, 192);
  box-shadow: none;
  border-top: solid rgb(0, 0, 0) 1.5px;
  border-left: solid rgb(0, 0, 0) 1.5px;
  border-bottom: solid rgb(250, 250, 250) 1.5px;
  border-right: solid rgb(250, 250, 250) 1.5px;
}

.badge-grid {
  display: table;
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

.subtitle {
  font-size: 12px;
  color: gray;
}

.heading {
  padding-bottom: 5px;
}

.inner-content {
  padding-top: 30px;
}

.inner-content:last-child {
  padding-bottom: 80px;
}

.fullscreen {
  width: 100% !important;
  height: var(--fullscreen) !important;
  margin: 0;
  transition: all 0.5s ease;
  padding: 0;
}

.nossaflex-app {
  max-width: 64px;
  max-height: 64px;
  border-radius: 22%;
  overflow: hidden;
  display: inline-block;
  vertical-align: middle;
  background-image: url("../assets/Icons/NossaflexLight.webp");
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  border: rgb(0, 0, 0, 0, 0.5) 1px solid;
}

.close {
  display: none;
}

.show {
  display: block;
}

.top-bar {
  display: flex;
  height: 25px;
  width: auto;
  background: rgb(0, 0, 124);
  z-index: 10;
  align-items: center;
  justify-content: space-between;
  flex-direction: row;
  margin: 2px;
}

.top-bar-deactivated {
  background: rgb(123, 125, 123);
}

.triple-button {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.button-red {
  height: 12px;
  width: 12px;
  border-radius: 50%;
  background: #ed6a06;
  display: flex;
  justify-content: center;
  align-items: center;
}

.button-yellow {
  height: 12px;
  width: 12px;
  border-radius: 50%;
  background: #f5bf50;
}

.button-green {
  height: 12px;
  width: 12px;
  border-radius: 50%;
  background: #62c454;
}

.button-red:hover {
  cursor: pointer;
}

.button-yellow:hover {
  cursor: pointer;
}

.button-green:hover {
  cursor: pointer;
}

.textarea-content {
  width: 100%;
  height: 100%;
  background: none;
  border: none;
  overflow: auto;
  outline: none;
  -webkit-box-shadow: none;
  -moz-box-shadow: none;
  box-shadow: none;
  resize: none;
  caret-color: black;
  color: black;
}

.bar {
  background: rgb(0, 0, 124);
  height: 1px;
  width: 100%;
}

.circle {
  background: #f1f0f2;
  width: 150px;
  height: 150px;
  border-radius: 50%;
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.05), 0 6px 20px 0 rgba(0, 0, 0, 0.05);
  display: flex;
  justify-content: center;
  align-items: center;
}

.content {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  justify-content: flex-start;
  height: 100%;
}

.header {
  font-weight: 700;
  font-size: 28px;
  padding-top: 10px;
}

.scroll-container {
  overflow: scroll;
  padding-left: 50px;
  padding-right: 50px;
  padding-top: 20px;
}

.expandedScrollContainer {
  padding-left: 25vw;
  padding-right: 25vw;
}

.paragraph {
  font-weight: 100;
  font-size: 14px;
  padding-bottom: 10px;
}

.paragraph:last-child {
  padding-bottom: 0px;
}

.resizer-r {
  cursor: col-resize;
  height: 100%;
  right: 0;
  top: 0;
  width: 5px;
}

.resizer-b {
  bottom: 0;
  cursor: row-resize;
  height: 5px;
  left: 0;
  width: 100%;
}

.resizer-t {
  top: 0;
  cursor: row-resize;
  height: 5px;
  left: 0;
  width: 100%;
}

.resizer-l {
  cursor: col-resize;
  height: 100%;
  left: 0;
  bottom: 0;
  width: 5px;
}

.resizer {
  position: absolute;
}
</style>

<script>
import interact from "interactjs";
export default {
  props: {
    // shownProp: Boolean
  },
  data: function () {
    return {
      resizeOption: {
        edges: { top: true, left: true, bottom: true, right: true },
      },
      positions: {
        clientX: undefined,
        clientY: undefined,
        movementX: 0,
        movementY: 0,
      },
      dragOption: {
        modifiers: [
          interact.modifiers.restrictRect({
            restriction: "parent",
            endOnly: true,
          }),
        ],
        allowFrom: ".top-bar",
      },

      // values for interact.js transformation
      x: 0,
      y: 0,
    };
  },
  computed: {
    style() {
      return {
        height: `${this.h}px`,
        width: `${this.w}px`,
        transform: `translate(${this.x}px, ${this.y}px)`,
        "--fullscreen": window.innerHeight - 40 + "px",
      };
    },
  },
  methods: {
    showPhotos(e) {
      e.stopPropagation();
      this.$store.commit("changeActiveWindow", "Photos");
      this.$store.commit("toggleShownPhotos", true);
      setTimeout(() => {
        this.$store.commit("zIndexIncrement", "photos");
      }, 1);
    },
    showColorization(e) {
      e.stopPropagation();
      this.$store.commit("changeActiveWindow", "Colorization");
      this.$store.commit("toggleShownColorization", true);
      setTimeout(() => {
        this.$store.commit("zIndexIncrement", "colorization");
      }, 1);
    },
    showNossaflex(e) {
      e.stopPropagation();
      this.$store.commit("changeActiveWindow", "NOSSAFLEX");
      this.$store.commit("toggleShownNossaflex", true);
      setTimeout(() => {
        this.$store.commit("zIndexIncrement", "noss");
      }, 1);
    },
    dragmove(event) {
      this.x += event.dx;
      this.y += event.dy;
      this.$store.commit("zIndexIncrement", "bio");
    },
    resizemove(event) {
      this.w = event.rect.width;
      this.h = event.rect.height;

      this.x += event.deltaRect.left;
      this.y += event.deltaRect.top;
    },
    dragMouseDown: function (event) {
      event.preventDefault();
      // get the mouse cursor position at startup:
      this.positions.clientX = event.clientX;
      this.positions.clientY = event.clientY;
      document.onmousemove = this.elementDrag;
      document.onmouseup = this.closeDragElement;
    },
    elementDrag: function (event) {
      event.preventDefault();
      this.positions.movementX = this.positions.clientX - event.clientX;
      this.positions.movementY = this.positions.clientY - event.clientY;
      this.positions.clientX = event.clientX;
      this.positions.clientY = event.clientY;
      // set the element's new position:
      this.$refs.draggableContainer.style.top =
        this.$refs.draggableContainer.offsetTop -
        this.positions.movementY +
        "px";
      this.$refs.draggableContainer.style.left =
        this.$refs.draggableContainer.offsetLeft -
        this.positions.movementX +
        "px";
    },
    closeDragElement() {
      document.onmouseup = null;
      document.onmousemove = null;
    },
    minimizeBio(e) {
      e.stopPropagation();
      this.$store.commit("toggleShownBio", false);
      this.$store.commit("changeActiveWindow", "Finder");
    },
    closeBio(e) {
      e.stopPropagation();
      this.$store.commit("toggleCloseBio", false);
      this.$store.commit("toggleShownBio", false);
    },
  },
  mounted: function () {
    // Query the element
    const ele = document.getElementById("container");

    // The current position of mouse
    let x = 0;
    let y = 0;

    // The dimension of the element
    let w = 0;
    let h = 0;

    const mouseDownHandlerRight = function (e) {
      x = e.clientX;

      const styles = window.getComputedStyle(ele);
      w = parseInt(styles.width, 10);

      document.addEventListener("mousemove", mouseMoveHandlerRight);
      document.addEventListener("mouseup", mouseUpHandlerRight);
    };

    const mouseDownHandlerLeft = function (e) {
      x = e.clientX;

      const styles = window.getComputedStyle(ele);
      w = parseInt(styles.width, 10);

      document.addEventListener("mousemove", mouseMoveHandlerLeft);
      document.addEventListener("mouseup", mouseUpHandlerLeft);
    };

    const mouseDownHandlerUp = function (e) {
      y = e.clientY;

      const styles = window.getComputedStyle(ele);
      h = parseInt(styles.height, 10);

      document.addEventListener("mousemove", mouseMoveHandlerUp);
      document.addEventListener("mouseup", mouseUpHandlerUp);
    };

    const mouseDownHandlerDown = function (e) {
      y = e.clientY;

      const styles = window.getComputedStyle(ele);
      h = parseInt(styles.height, 10);

      document.addEventListener("mousemove", mouseMoveHandlerDown);
      document.addEventListener("mouseup", mouseUpHandlerDown);
    };

    const mouseMoveHandlerUp = function (e) {
      // How far the mouse has been moved
      const dy = e.clientY - y;

      // Adjust the dimension of element
      ele.style.height = `${h - dy}px`;
    };

    const mouseMoveHandlerDown = function (e) {
      // How far the mouse has been moved
      const dy = e.clientY - y;

      // Adjust the dimension of element
      ele.style.height = `${h + dy}px`;
    };

    const mouseMoveHandlerRight = function (e) {
      // How far the mouse has been moved
      const dx = e.clientX - x;

      // Adjust the dimension of element
      ele.style.width = `${w + dx}px`;
    };

    const mouseMoveHandlerLeft = function (e) {
      // How far the mouse has been moved
      const dx = e.clientX - x;

      // Adjust the dimension of element
      ele.style.width = `${w - dx}px`;
    };

    const mouseUpHandlerUp = function () {
      // Remove the handlers of `mousemove` and `mouseup`
      document.removeEventListener("mousemove", mouseMoveHandlerUp);
      document.removeEventListener("mouseup", mouseUpHandlerUp);
    };

    const mouseUpHandlerDown = function () {
      // Remove the handlers of `mousemove` and `mouseup`
      document.removeEventListener("mousemove", mouseMoveHandlerDown);
      document.removeEventListener("mouseup", mouseUpHandlerDown);
    };

    const mouseUpHandlerRight = function () {
      // Remove the handlers of `mousemove` and `mouseup`
      document.removeEventListener("mousemove", mouseMoveHandlerRight);
      document.removeEventListener("mouseup", mouseUpHandlerRight);
    };

    const mouseUpHandlerLeft = function () {
      // Remove the handlers of `mousemove` and `mouseup`
      document.removeEventListener("mousemove", mouseMoveHandlerLeft);
      document.removeEventListener("mouseup", mouseUpHandlerLeft);
    };
    // Query all resizers
    const resizersRight = ele.querySelectorAll(".resizer-r");
    const resizersUp = ele.querySelectorAll(".resizer-t");
    const resizersDown = ele.querySelectorAll(".resizer-b");
    const resizersLeft = ele.querySelectorAll(".resizer-l");

    [].forEach.call(resizersRight, function (resizer) {
      resizer.addEventListener("mousedown", mouseDownHandlerRight);
    });

    [].forEach.call(resizersUp, function (resizer) {
      resizer.addEventListener("mousedown", mouseDownHandlerUp);
    });

    [].forEach.call(resizersDown, function (resizer) {
      resizer.addEventListener("mousedown", mouseDownHandlerDown);
    });

    [].forEach.call(resizersLeft, function (resizer) {
      resizer.addEventListener("mousedown", mouseDownHandlerLeft);
    });
  },
};
</script>
