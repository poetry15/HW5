<template>
  <div class="line_box">
    <div class="line"></div>
    <div class="or">或</div>
    <div class="line"></div>
  </div>
</template>

<script>
export default {
}
</script>

<style scoped>
.line_box {
  display: flex;
  flex-direction: row;
  margin: 10px 40px 18px;
}

.line {
  top: 0.45em;
  flex-shrink: 1;
  height: 1px;
  width: 80px;
  position: relative;
  flex-grow: 1;
  background-color: rgb(219,219,219);
}

.or {
  display: flex;
  margin-right: 18px;
  margin-bottom: 0;
  flex-direction: column;
  margin-left: 18px;
  font-size: .8125rem;
  align-items: stretch;
}
</style>