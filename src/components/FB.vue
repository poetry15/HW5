<template>
  <button class="FB" type="button" @click="FB_login">
    <span class="logo"></span>
    <span style="color: #385185">使用 Facebook 帳號登入</span>
  </button>
</template>

<script>
export default {
  methods: {
    FB_login() {
      alert("FB登入正在維修中，請輸入帳號與密碼")
    }
  }
};
</script>

<style scoped>
.FB {
  background: none;
  border: none;
  cursor: pointer;
  color: rgb(0,149,246);
  margin-bottom: 40px;
  font-weight: 600;
  font-size: 15px;
}

.logo {
  background-image: url("FB.png");
  background-repeat: no-repeat;
  background-position: -414px -259px;
  height: 16px;
  width: 16px;
  display: inline-block;
  font: inherit;
  font-size: 100%;
  margin-right: 8px;
  padding: 0;
  position: relative;
  top: 3px;
  vertical-align: baseline;
}
@media (min-device-pixel-ratio: 1.5), (min-resolution: 144dpi) {
  .logo {
    background-size: 440px 411px;
    background-position: -347px -329px;
  }
}
</style>