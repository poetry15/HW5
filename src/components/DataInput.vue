<template>
    <div class="data">
      <label class="input">
        <span class="hint">手機號碼、用戶名稱或電子郵件地址</span>
        <input type="text" id="login" name="login" value>
      </label>
      <label class="input">
        <span class="hint">密碼</span>
        <input type="password" id="password" name="password" value>
      </label>
    </div>
    <button class="login_btn" type="submit" @click="login">登入</button>
</template>

<script>
export default {
  methods: {
    login() {
      alert("請確認登入!!!");
      setTimeout(() => {
        location.href = 'next.html';
      }, 2000);
    }
  }
};
</script>

<style scoped>
.input {
  margin: 0 40px 6px;
  border: 0;
  display: flex;
  flex: 1 0 0;
  font: inherit;
  font-size: 100%;
  height: 36px;
  min-width: 0;
  position: relative;
  vertical-align: baseline;
}

input[type="text"] , input[type="password"]{
  border-top: 1px solid rgb(219,219,219);
  border-bottom: 1px solid rgb(219,219,219);
  border-left: 1px solid rgb(219,219,219);
  border-right: 1px solid rgb(219,219,219);
  outline: none;
  font-size: 17px;
  padding: 14px 0 2px 8px;
}

.hint {
  color: rgb(115,115,155);
  font-size: 13px;
  height: 36px;
  left: 8px;
  line-height: 36px;
  margin: 0;
  overflow: hidden;
  position: absolute;
  transform-origin: left;
  transform: scale(calc(10 / 12)) translateY(-10px);
}

.data {
  margin-top: 24px;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.login_btn {
  background-color: rgba(0,149,246);
  color: rgb(255,255,255);
  border-radius: 8px;
  opacity: .7;
  position: relative;
  border: none;
  box-sizing: border-box;
  width: 219px;
  padding: 7px 16px;
  margin-bottom: 8px;
  cursor: pointer;
  font-weight: 600;
}

.login_btn:hover {
  background-color: rgba(24,119,242);
}
</style>
