<template>
  <header style="background-color:gray;">
    <h2>header</h2>
  </header>
  <div id="body">
    <div id="left">
      <h2>#left</h2>
    </div>
    <div id="center">
      <h2>#center</h2>
    </div>
    <div id="right">
      <h2>#right</h2>
    </div>
  </div>
  <footer>
    <h2>#footer</h2>
  </footer>
</template>

<script>
export default {
  name: "HolyGrailLayout"
}
</script>

<style scoped>
.sb {
  display: flex;
  min-height: 100vh;
  flex-direction: column;
}

header, footer {

  flex: 1;
}
#body{
  display: flex;
}
#center{
  display: flex;
  flex: 1;
  justify-content: center;
  background-color: aqua;
}
#left, #right {
  flex: 0 0 12em;
}
#left{
  order: -1;
}
footer{
  display: flex;
  justify-content: center;
}
</style>