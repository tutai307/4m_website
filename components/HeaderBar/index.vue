<template lang="pug">
  div
    //.header-top.main-color

    v-container.main-font-size
      v-row.max-width
        v-col(cols="6" md="3")
          v-img(src="/logo.jpg" max-width="120" )
        v-col.pc(cols="6" md="9")
          ul.pt-2.hidden-sm-and-down
            li.pa-2(@click="$router.push({path: 'contact'})") Contact
            li.pa-2(@click="$router.push({path: 'about_us'})") About Us
            li.pa-2(@click="$router.push({path: '/'})") Home
          v-icon.hidden-md-and-up.pt-2(style="float: right" @click="onShowCategory") mdi-menu
      .center.hidden-md-and-up
        v-expand-transition
          v-card(
            v-show="isShowCategoryInMobile"
            class="mx-auto"
          )
            ul
              li.pa-2(@click="$router.push({path: 'contact'})") Contact
              li.pa-2(@click="$router.push({path: 'about_us'})") About Us
              li.pa-2(@click="$router.push({path: '/'})") Home             
    v-carousel(hide-delimiters)
      v-carousel-item
        v-img.banner(src="/2023-01-12_18-15.png" height="450px" cover)
      v-carousel-item
        v-img.banner(src="/IMG-Full-width-1536x481.jpg" height="450px" cover)
      v-carousel-item
        v-img.banner(src="/2. Southall shed 2 1800 px.jpg" height="450px" cover)
</template>

<script>
const HeaderBar = {
  data() {
    return {
      isShowCategoryInMobile: false
    }
  },
  methods: {
    onShowCategory() {
      this.isShowCategoryInMobile = !this.isShowCategoryInMobile
    },
  }
}

export default HeaderBar
</script>

<style scoped>
/* Trong file CSS/SCSS của bạn */
.center {
  margin: 0 auto;
  text-align: center;
}

.max-width {
  max-width: 1300px;
  margin: 0 auto;
}

.main-color {
  background-color: #e8ca74;
}

.header-top {
  height: 30px;
  width: 100%;
}

.margin-bottom-1 {
  margin-bottom: 1px;
}

.pc ul li {
  list-style: none;
  float: right;
  padding-left: 2rem;
  cursor: pointer;
}

.navbar-brand {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  font-size: 35px;
  color: #9ec2bb;
}

@media only screen and (max-width: 1378px) {
  .banner {
    height: 450px;
  }
}

.main-font-size {
  font-size: 22px;
}
</style>