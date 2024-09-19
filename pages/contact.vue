<template lang="pug">
  div
    header-bar
    
    v-container.max-width
      h1.center.main-color.pt-5.hidden-sm-and-down CONTACT
      v-divider
      v-row.pt-5
        v-col(cols="12" md="6")
          iframe(
                src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3488.2008952946703!2d105.77029538055774!3d21.03581550098388!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x313454b782649e49%3A0x8a2c947e0d4710d4!2zNyDEkC4gTMOqIMSQ4bupYyBUaOG7jSwgTeG7uSDEkMOsbmgsIFThu6sgTGnDqm0sIEjDoCBO4buZaSwgVmnhu4d0IE5hbQ!5e0!3m2!1svi!2s!4v1673669733910!5m2!1svi!2s"
                width="100%" height="450" style="border:0;" allowfullscreen="" loading="lazy"
                referrerpolicy="no-referrer-when-downgrade")
        v-col(cols="12" md="6")
          p.high-light.pa-2.pt-5 Head office
          v-divider
          p.pa-2 Address No 7/9 Le Duc Tho, My Dinh 2, Nam Tu Lien, Hanoi
          p.pa-2 Phone: (024) 7102 6888
          p.pa-2 Hotline: (024) 7102 6888
          p.pa-2 Email: services1@4mvietnam.com.vn
          p.pa-2 Email: services2@4mvietnam.com.vn
    footer-bar
</template>

<script>
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
.high-light {
  font-size: 25px;
  color: #111111;
}
.main-color {
  color: #275199;
}
</style>