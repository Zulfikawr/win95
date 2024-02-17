<template>
  <div class="menu" style="z-index: 1000000">
    <div class="sidebar">
      <img class="sidebar-image" src="@/assets/icons/win95icons/sidebar-image.png" />
    </div>
    <div class="socials">

      <a
        href="https://www.linkedin.com/in/muhammad-zulfikar-076a7b227"
        target="_blank">
        <div class="bar">
          <img class="social-image" src="@/assets/icons/win95icons/social/linkedin.png" />
          <u>L</u>inkedIn
        </div>
      </a>

      <a href="https://github.com/muhammad-zulfikar" target="_blank">
        <div class="bar">
          <img class="social-image" src="@/assets/icons/win95icons/social/github.svg" />
          <u>G</u>itHub
        </div>
      </a>

      <a href="https://wa.me/+6285156453730" target="_blank">
        <div class="bar">
          <img
            class="social-image"
            src="@/assets/icons/win95icons/social/whatsapp.png"
          />
          <div class="social-text"><u>W</u>hatsApp</div>
        </div>
      </a>

      <a href="https://telegram.com/spookies/" target="_blank">
        <div class="bar">
          <img class="social-image" src="@/assets/icons/win95icons/social/telegram.png" />
          <u>T</u>elegram
        </div>
      </a>      

      <a href="https://www.kaggle.com/zulfikarmuhammad/" target="_blank">
        <div class="bar">
          <img class="social-image" src="@/assets/icons/win95icons/social/kaggle.png" />
          <u>K</u>aggle
        </div>
      </a>

      <a href="/files/don_chia_resume.pdf" target="_self">
        <div class="bar">
          <img class="social-image" src="@/assets/icons/win95icons/text.png" />
          <u>R</u>ésumé
        </div>
      </a>

      <div class="divider"></div>

      <a href="javascript:window.close();" target="_self">
        <div class="bar">
          <img class="social-image" src="@/assets/icons/win95icons/shutdown.png" />
          <u>S</u>hut Down...
        </div>
      </a>

    </div>
  </div>
</template>
<style scoped>
.menu {
  width: 165px;
  height: 282px;
  background: black;
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
  display: flex;
  flex-direction: row;
  align-items: flex-start;
  font-size: 12px;
}

a {
  color: black;
  text-decoration: none;
}

.sidebar {
  width: 25px;
  background: rgb(123, 125, 123);
  height: 100%;
  display: flex;
  align-items: flex-end;
}

.sidebar-image {
  width: 100%;
}

@media only screen and (max-width: 600px) {
  .sidebar {
    width: 25px;
    background: rgb(123, 125, 123);
    height: 100%;
    display: flex;
    align-items: flex-end;
  }
}

.divider {
  width: 100%;
  height: 1px;
  background: rgb(123, 125, 123);
  border-bottom: white solid 1px;
}

.socials {
  flex-grow: 1;
}

.social-image {
  width: 30px;
  height: 30px;
  margin-right: 10px;
  border-radius: 6px;
}

.bar {
  display: flex;
  flex-direction: row;
  padding: 5px 10px 5px 10px;
  align-items: center;
}

.bar:hover {
  background: rgb(0, 0, 118);
  color: white;
}
</style>
<script>
export default {};
</script>
