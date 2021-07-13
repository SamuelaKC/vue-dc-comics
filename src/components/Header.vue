<template>
  <div class="container">
    <div class="content">
      <div class="logo">
        <img src="../assets/dc-logo.png" alt="logo dc" />
      </div>
      <div class="navbar">
        <ul>
          <li v-for="element in LinksMenu" :key="element.id">
            <a :href="element.link">{{ element.name }}</a>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Header',
  data: function () {
    return {
      LinksMenu: [
        {
          id: 0,
          href: '#',
          name: 'CHARACTERS',
        },
        {
          id: 1,
          href: '#',
          name: 'COMICS',
        },
        {
          id: 2,
          href: '#',
          name: 'MOVIES',
        },
        {
          id: 3,
          href: '#',
          name: 'TV',
        },
        {
          id: 4,
          href: '#',
          name: 'GAMES',
        },
        {
          id: 5,
          href: '#',
          name: 'COLLECTIBLES',
        },
        {
          id: 6,
          href: '#',
          name: 'VIDEOS',
        },
        {
          id: 7,
          href: '#',
          name: 'FANS',
        },
        {
          id: 8,
          href: '#',
          name: 'NEWS',
        },
        {
          id: 9,
          href: '#',
          name: 'SHOP',
        },
      ],
    }
  },
}
</script>

<style lang="scss" scoped>
@import '../style/colors.scss';
@import '../style/fonts.scss';

.content {
  margin-top: 50px;
  margin-bottom: 10px;

  .logo {
    width: 40%;
    text-align: center;
  }

  .navbar {
    flex-grow: 1;
    display: flex;

    ul {
      display: flex;
      list-style: none;
      justify-content: center;
      font-size: 14px;
      font-weight: 700;

      li {
        padding: 0 10px;

        a {
          color: $header-link-color;
          text-decoration: none;
          &:hover {
            color: $link-color;
            padding-bottom: 50px;
            border-bottom: 5px solid $bg-color-blue;
            cursor: pointer;
          }
        }
      }
    }
  }
}
</style>
