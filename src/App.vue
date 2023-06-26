<template>
  <div class="app">
    <AppHeader :navDropdown="header.dropdowns" :navLi="header.li" :navMenuLi=header.list />
    <AppMain />
    <AppFooter :aboutUs=footer.aboutUs :movieCategory=footer.movieCategory :information=footer.information
      :recentPosts=footer.recentPosts :footerBottomNav=footer.footerBottomNav :socialIcons=footer.aboutUs.socialIcons />

  </div>
</template>

<script>
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import AppFooter from './components/AppFooter.vue'

export default {
  name: 'App',
  components: {
    AppHeader,
    AppMain,
    AppFooter,
  },
  data() {
    return {
      header: {
        dropdowns: [{
          name: 'Home',
          list: ['home', 'home1', 'home2', 'home3', 'home4', 'home5', 'home6']
        },
        {
          name: 'Celebrity',
          list: ['Celebrity', 'Celebrity Single']
        },
        {
          name: 'Movie',
          list: ['Movie Post', 'Top Rate Movies', 'Movie Category', 'Single Movie']
        },
        {
          name: 'Page',
          list: ['Pricing Table', 'Call To Action', 'My Account', 'Cart', 'Checkout', 'Wishlist']
        },
        {
          name: 'Shop',
          list: ['Shop Sidebar', 'No Sidebar']
        },
        ],
        li: [
          'Blog', 'Contact Us'
        ]
      },

      footer: {
        aboutUs: {
          text: 'Mauris malesuada arcu eu posuere eleifen. Ut egestas tortor at leo egestas tincidunt. Nam tincidunt metus tristique tristique viverra. Mauris erat ante, egestas vitae dapibus seds.',
          socialIcons: [
            'fa-brands fa-facebook-f', 'fa-brands fa-twitter', 'fa-brands fa-linkedin-in', 'fa-brands fa-instagram', 'fa-brands fa-pinterest'
          ],
          colors: [
            ''
          ]
        },
        movieCategory: [
          {
            name: 'English New Movie',
            link: ' #'
          },
          {
            name: 'Hindi All Movie',
            link: '#'
          },
          {
            name: 'Latest Tamil Movie',
            link: '#'
          },
          {
            name: 'New Top Rating Movie',
            link: '#'
          },
          {
            name: 'Hornn New movie',
            link: '#'
          },
          {
            name: 'Animation New Movie',
            link: '#'
          },

        ],
        information: [
          {
            name: 'Youtube video Post',
            link: ' #'
          },
          {
            name: 'Actor Information',
            link: '#'
          },
          {
            name: 'New Promotion',
            link: '#'
          },
          {
            name: 'Latest Movie In English',
            link: '#'
          },
          {
            name: 'Latest Flim Product',
            link: '#'
          },
          {
            name: 'Video New Video',
            link: '#'
          },
        ],
        recentPosts: [
          {
            img: '../../public/blog-100x100.jpg',
            title: 'Actor The Concept Movie High Concept Theory see ',
            date: 'April 14, 2020'
          },
          {
            img: '../../public/blog2-100x100.jpg',
            title: 'consequat Nam lectus nibh aucibus It has turpis',
            date: 'April 14, 2020'
          },
          {
            img: '../../public/blog3-100x100.jpg',
            title: 'Nam lectus nibh consequat aucibus turpis',
            date: 'April 14, 2020'
          }
        ],
        footerBottomNav: [
          'Tram And Conditions',
          'Policy',
          'About'
        ]
      }
    }
  },
}
</script>
<style lang="scss">
@import './styles/general.scss';
@import './styles/partials/variables';
@import "bootstrap/scss/bootstrap";

div.app {
  font-family: 'Roboto', sans-serif;
  background-color: $colorSecondary;
  color: $colorLight;
}
</style>
