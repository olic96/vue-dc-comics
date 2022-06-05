<template>
 <div class="container">
    <header class="header">
      <div class="header__logo">
          <img src="../assets/img/dc-logo.png">
      </div>
      <nav class="header__nav" >
        <ul>
          <li v-for="(link, index) in nav" :key="index" :class="{active : link.isActive}" @click="active(index)">
            <a href="#">{{link.text}}</a>
          </li>
        </ul>
      </nav>
  </header>
 </div>
</template>

<script>
export default {
        name: 'BaseHeader',
        data() {
            return {
                nav: [
                    {
                        text: "Characters",
                        href: "#",
                        isActive: false,
                    },
                    {
                        text: "Comics",
                        href: "#",
                        isActive: true,
                    },
                    {
                        text: "Movie",
                        href: "#",
                        isActive: false,
                    },
                    {
                        text: "Tv",
                        href: "#",
                        isActive: false,
                    },
                    {
                        text: "Games",
                        href: "#",
                        isActive: false,
                    },
                    {
                        text: "Collectibles",
                        href: "#",
                        isActive: false,
                    },
                    {
                        text: "Videos",
                        href: "#",
                        isActive: false,
                    },
                    {
                        text: "Fans",
                        href: "#",
                        isActive: false,
                    },
                    {
                        text: "News",
                        href: "#",
                        isActive: false,
                    },
                    {
                        text: "Shop",
                        href: "#",
                        isActive: false,
                    },
                ],
            }
        },
      methods: {
        active(index) {
          this.nav.forEach(link => {
            link.isActive = false;
          });
          this.nav[index].isActive = !this.nav[index].isActive;
        }
      }
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

      .active a {
        color: var(--primary-color);
        border-color: var(--primary-color);
      }
    }
  }
</style>