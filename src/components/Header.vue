<template>
  <div class="main">
    <nav class="navbar navbar-expand-lg">
      <div class="container-fluid">
        <div class="navbar__header">
          <a href="#"
            ><img
              class="navbar__header--logo"
              src="../assets/logo/logo.png"
              alt="logo"
          /></a>
          <a href="#"
            ><img
              class="navbar__header--menu"
              src="../assets/icon/menu.png"
              alt="logo"
          /></a>
        </div>
      </div>
    </nav>
  </div>
</template> 

<script>
export default {};
</script>

<style scoped>
.main {
  background-color: #2698fb6b;
}
.container-fluid {
  display: block;
}
.navbar__header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0 80px;
}
</style>