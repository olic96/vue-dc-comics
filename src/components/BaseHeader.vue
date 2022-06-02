<template>
 <div class="container">
    <header class="header">
      <div class="header__logo">
          <img src="../assets/img/dc-logo.png">
      </div>
      <nav class="header__nav">
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

    &__nav {
        ul {
          display: flex;
          list-style-type: none;
          font-size: 1.25rem;

          a {
            display: inline-block;
            text-decoration: none;
            padding: 1.875rem 0.9375rem;
            color: var(--secondary-color);
            border-bottom: 0.3125rem solid transparent;;
          }

          :hover a {
            color: var(--primary-color);
            border-color: var(--primary-color);
          }
        }
    }
   
  }
</style>