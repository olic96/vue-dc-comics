<template>
 <div class="container">
    <header class="header">
      <div class="logo">
          <img src="../assets/img/dc-logo.png">
      </div>
      <nav class="header-nav">
        <ul>
          <li><a href="#">link</a></li>
          <li><a href="#">link</a></li>
          <li><a href="#">link</a></li>
          <li><a href="#">link</a></li>
          <li><a href="#">link</a></li>
          <li><a href="#">link</a></li>
          <li><a href="#">link</a></li>
          <li><a href="#">link</a></li>
          <li><a href="#">link</a></li>
          <li><a href="#">link</a></li>
        </ul>
      </nav>
  </header>
 </div>
</template>

<script>
export default {
  name: 'BaseHeader',

}
</script>

<style lang="scss" scoped>
  .header{
    display: flex;
    justify-content: space-between;
  }
</style>