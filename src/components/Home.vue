<template>
  <div>
    <section id="hero">
      <div class="hero container">
        <div>
          <h1>Share your <span></span></h1>
          <h1>holiday dream <span></span></h1>
          <h3>And find the perfect partner to fulfill it <span></span></h3>

          <div class="btn-findpatner">
            <v-btn rounded small color="#FF4E50" class="btn-findpatner" dark
              >Find your holiday partner</v-btn
            >
          </div>
        </div>
      </div>
    </section>

    <div class="block">
      <h2 class="text-center meeting_header">
        Meet a partner for your best holiday
      </h2>
      <v-container class="avatars">
        <v-row>
          <v-col v-for="item in items" :key="item.id" cols="12" sm="6" md="3"
            ><v-card flat class="mx-auto avatarCard">
              <v-img class="partner_img" :src="item.src"> </v-img>

              <v-card-text class="text--primary">
                <h4 class="fullname">{{ item.name }}</h4>
                <p class="desc">{{ item.title }}</p>
              </v-card-text>
            </v-card></v-col
          >
        </v-row>
      </v-container>
      <div class="btn-more">
        <v-btn rounded class="ma-2 btn-more" outlined>See other patners</v-btn>
      </div>
    </div>

    <div class="block">
      <h2 class="text-center discover_header">
        Discover holiday activity ideas
      </h2>
      <div class="images_conatiner">
        <div class="card">
          <img src="../assets/block1Sports.jpg" alt="" />
          <div class="centered_text">Sports</div>
        </div>
        <div class="card">
          <img src="../assets/block2Wellness.jpg" alt="" />
          <div class="centered_text">Wellness and Health</div>
        </div>
        <div class="card">
          <img src="../assets/block3Expeditions.jpg" alt="" />
          <div class="centered_text">Expeditions</div>
        </div>
        <div class="card">
          <img src="../assets/block4Games.jpg" alt="" />
          <div class="centered_text">Games</div>
        </div>
        <div class="card">
          <img src="../assets/block5Culture.jpg" alt="" />
          <div class="centered_text">Culture and Education</div>
        </div>
        <div class="card">
          <img src="../assets/block6Beauty.jpg" alt="" />
          <div class="centered_text">Beauty and Relaxation</div>
        </div>
        <div class="card">
          <img src="../assets/block7Travelling.jpg" alt="" />
          <div class="centered_text">Travelling</div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Home',

  data () {
    return {
      items: [
        {
          id: 1,
          src: require('../assets/partner1.jpg'),
          name: 'Bradly Hunter',
          title: 'Base in Chicago. I love paying tennis and loud music'
        },
        {
          id: 2,
          src: require('../assets/partner2.jpg'),
          name: 'Marie Bennett',
          title:
            'Current living in Colorado. Lover of art, languages and travelling'
        },
        {
          id: 3,
          src: require('../assets/partner3.jpg'),
          name: 'Diana Wells',
          title:
            'Living in Athens, Greece, I love black and white classics, chillout music and green tea'
        },
        {
          id: 4,
          src: require('../assets/partner4.jpg'),
          name: 'Chrispher Pierce',
          title:
            'Star wars fanatic. I have a persistent enthusiasm to create new things'
        }
      ]
    }
  }
}
</script>
<style scoped>
.container {
  min-height: 100vh;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
}

.avatars {
  min-height: 0vh;
}
.brand h1 {
  font-size: 1.5rem;
  text-transform: uppercase;
  color: white;
}

#hero {
  background-image: url(../assets/headerBackground.jpg);
  background-size: cover;
  background-position: top center;
  position: relative;
  z-index: 1;
}
#hero::after {
  content: "";
  position: absolute;
  left: 0;
  top: 0;
  height: 100%;
  width: 100%;
  background-color: black;
  opacity: 0.3;
  z-index: -1;
}
#hero .hero {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 50px;
  justify-content: center;
}
#hero h1 {
  display: block;
  width: fit-content;
  font-size: 2rem;
  position: relative;
  color: #fff;
  text-transform: uppercase;
  margin: 0 auto;
  text-align: center;
}
#hero h3 {
  display: block;
  width: fit-content;
  font-size: 1.2rem;
  margin: 0 auto;
  position: relative;
  color: #fff;
  text-align: center;
}

.v-card > *:first-child:not(.v-btn):not(.v-chip),
.v-card > .v-card__progress + *:not(.v-btn):not(.v-chip) {
  border-radius: 50%;
}
.partner_img {
  border-radius: 50%;
  width: 60%;
  margin-left: 23%;
}
.fullname,
.desc {
  text-align: center;
}
.desc {
  color: #666666;
}
.block {
  padding: 5px;
}

.meeting_header {
  padding: 30px 0 0 0;
  color: #444444;
  font-weight: lighter;
  font-size: 22px;
}
.discover_header {
  padding: 50px 0;
}
.btn-more {
  justify-content: center !important;
  display: flex !important;
  align-items: center !important;
  color: #ff4e50 !important;
  text-transform: initial;
}
.btn-findpatner {
  justify-content: center !important;
  display: flex !important;
  align-items: center !important;
  text-transform: initial !important;
  padding: 50px;
}

img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.images_conatiner {
  max-width: 1200px;
  margin: 0 auto;
  display: grid;
  grid-gap: 1rem;
  padding: 0 20px;
}
.card {
  position: relative;
  text-align: center;
  color: #fff;
  font-size: 20px;
  font-weight: 500;
  background: #fff;
  padding: 0rem;
}
.card:hover {
  color: #444444;
}

.centered_text {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
@keyframes hamburger_puls {
  0% {
    opacity: 1;
    transform: scale(1);
  }
  100% {
    opacity: 0;
    transform: scale(1.4);
  }
}
@media screen and (max-width: 1085px) {
  .footer-items {
    width: 50%;
  }
}
@media screen and (max-width: 600px) {
  .footer-items {
    width: 100%;
  }
}

/* Media Query For Tablet */
@media only screen and (min-width: 768px) {
  .cta {
    font-size: 2.5rem;
    padding: 20px 60px;
  }
  h1.section-title {
    font-size: 6rem;
  }

  /* Hero */
  #hero h1 {
    font-size: 3rem;
  }
  /* End Hero */
}
/* End Media Query For Tablet */

/* Media Query For Desktop */
@media only screen and (min-width: 1200px) {
  .images_conatiner {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-gap: 0.5rem;
  }
  .card:nth-child(5) {
    grid-column: span 2;
  }
  .card:nth-child(6) {
    grid-column: span 2;
  }
  p {
    font-size: 12px;
  }
  .meeting_header {
    padding: 50px 0 0 0;
  }
  /* header */
  #header .hamburger {
    display: none;
  }
  #header .nav-list ul {
    position: initial;
    display: block;
    height: auto;
    overflow: hidden;
    width: fit-content;
    background-color: transparent;
  }
  #header .nav-list ul li {
    display: inline-block;
  }
  #header .nav-list ul li a {
    font-size: 1rem;
  }
  #header .nav-list ul a:after {
    display: none;
  }
  #hero h1 {
    display: block;
    width: fit-content;
    font-size: 3rem;
    position: relative;
    color: #fff;
    text-transform: uppercase;
    margin: 0 auto;
    text-align: center;
  }
  #hero h3 {
    display: block;
    width: fit-content;
    font-size: 1.2rem;
    margin: 0 auto;
    position: relative;
    color: #fff;
    text-align: center;
  }
  .avatarCard {
    padding: 20px;
  }
  .block {
    padding: 0 180px;
  }
  /* End header */
}
/* End  Media Query For Desktop */
</style>
