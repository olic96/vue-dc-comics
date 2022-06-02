<template>
  <footer>
      <div class="container">
          <div class="footer-top">
             <div class="footer-top__item">
                <img class="footer-top__item-img" src="../assets/img/buy-comics-digital-comics.png">
                <p>DIGITAL COMICS</p>
             </div>
             <div class="footer-top__item">
                <img class="footer-top__item-img" src="../assets/img/buy-comics-merchandise.png">
                <p>DC MERCHANDISE</p>
             </div>
             <div class="footer-top__item">
                <img class="footer-top__item-img" src="../assets/img/buy-comics-subscriptions.png">
                <p>SUBSCRIPTIONS</p>
             </div>
             <div class="footer-top__item">
                <img class="footer-top__item-img" src="../assets/img/buy-comics-shop-locator.png">
                <p>COMICS SHOP LOCATOR</p>
             </div>
             <div class="footer-top__item">
                <img class="footer-top__item-img" src="../assets/img/buy-dc-power-visa.svg">
                <p>DC POWER PISA</p>
             </div>
          </div>
          <div class="footer__mid"></div>
          <div class="footer__bottom"></div>
      </div>
  </footer>
</template>

<script>
export default {
    name: 'BaseFooter',
}
</script>

<style lang="scss" scoped>
    footer {
        background-color: var(--primary-color);
         padding: 1.875rem;
    }
    .footer-top {
        display: flex;
        justify-content: space-around;
        align-items: center;

        &__item {
            display: flex;
            align-items: center;
            cursor: pointer;

            &-img {
            height: 2.1875rem;
            margin-right: 0.9375rem;
            }
        }

        p {
            color: #fff;
        }
        
    }
</style>