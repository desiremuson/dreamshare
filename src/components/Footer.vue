<template>
  <div class="footer">
    <div class="inner-footer">
      <div class="footer-items">
        <h1>DREAMSHARE</h1>
      </div>
      <div class="footer-items">
        <h2>Company</h2>
        <div class="border"></div>
        <ul>
          <a href=""><li>About</li></a>
          <a href=""><li>Contact</li></a>
          <a href=""><li>Press</li></a>
          <a href=""><li>Blog</li></a>
          <a href=""><li>Terms and Privacy</li></a>
          <a href=""><li>Help</li></a>
        </ul>
      </div>
      <div class="footer-items">
        <h2>Activities</h2>
        <div class="border"></div>
        <ul>
          <a href=""><li>Sports</li></a>
          <a href=""><li>Wellness and Health</li></a>
          <a href=""><li>Expeditions</li></a>
          <a href=""><li>Games</li></a>
          <a href=""><li>View all</li></a>
        </ul>
      </div>
      <div class="footer-items">
        <h2>Contact us</h2>
        <div class="border"></div>
        <ul>
          <a href=""><li>Tel: (+27) 614 529 157</li></a>
          <a href=""><li>Email: desiremuson@outlook.com</li></a>
        </ul>
      </div>
    </div>
  </div>
</template>
<style scoped>
h5 {
  margin-bottom: 10px !important;
}
.mx-auto {
  background-color: transparent !important;
  padding: 0 50px;
}

.footer {
  width: 100%;
  display: block;
  border-top: 3px solid #ff4e50;
  margin: 50px 20px 0 20px;
}
.inner-footer {
  width: 95%;
  margin: auto;
  padding: 30px 10px;
  display: flex;
  flex-wrap: wrap;
  box-sizing: border-box;
  justify-content: center;
}
.footer-items {
  width: 20%;
  padding: 10px 20px;
  box-sizing: border-box;
}
h1 {
  padding: 10px 0;
  font-size: 25px;
  color: #ff4e50;
  text-transform: uppercase;
}
.footer-items p {
  color: grey;
  font-size: 16px;
  text-align: justify;
  line-height: 25px;
}
h2 {
  margin: 10px 0;
  color: #444;
  font-weight: lighter;
}
.border {
  height: 2px;
  width: 40px;
}
ul {
  list-style: none;
  color: #fff;
  font-size: 15px;
  letter-spacing: 0.5px;
}
ul a {
  text-decoration: none;
  outline: none;
  color: #666;
  transition: 0.3s;
}
ul a:hover {
  color: #ff4e50;
}
ul li {
  margin: 10px 0;
  height: 25px;
}
li i {
  margin-right: 20px;
}
.social-media {
  width: 100%;
  color: #fff;
  text-align: center;
}
.social-media a {
  text-decoration: none;
}
.social-media i {
  height: 15px;
  width: 15px;
  margin: 20px 5px;
  padding: 10px;
  color: #fff;
  border-radius: 50%;

  transition: 0.3s;
}
.social-media i:hover {
  padding: 10px;

  color: #fff;
  font-size: 12px;
}
.footer-bottom {
  padding: 10px;
  background: #3d545f;
  color: #fff;
  font-size: 12px;
  text-align: center;
}
/* Keyframes */
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
</style>
