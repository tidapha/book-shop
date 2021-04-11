<template>
  <div id="app">
    <link
      href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.0-beta3/dist/css/bootstrap.min.css"
      rel="stylesheet"
      integrity="sha384-eOJMYsd53ii+scO/bJGFsiCZc+5NDVN2yr8+0RDqr0Ql0h+rP48ckxlpbzKgwra6"
      crossorigin="anonymous"
    />
    <link
      rel="stylesheet"
      href="../node_modules/owl.carousel/dist/assets/owl.carousel.min.css"
    />
    <div id="nav">
      <router-link to="/">ข้อ 1 - Basic Javascript (เลือกทำ 2 ข้อ)</router-link>
      || &nbsp;
      <router-link to="/two">ข้อ 2 - Database Design </router-link>
      || &nbsp;
      <router-link to="/three"
        >ข้อ 3 - ทำโจทย์ตามตำแหน่งที่ตนเองสมัคร</router-link
      >
    </div>
    <router-view />
  </div>
</template>

<style>
router-link,
a {
  text-decoration: none !important;
  color: unset !important;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}

.owl-theme .owl-nav {
  background: transparent !important;
}

.owl-prev,
.owl-next {
  font-size: 2.5rem !important;
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
}

.owl-prev {
  top: 50.5%;
  left: -0.7rem;
  width: 30px;
}

.owl-next {
  right: 0.5rem;
  width: 30px;
}

.owl-carousel .owl-stage {
  padding-bottom: 10px;
}

.owl-carousel .owl-nav button.owl-next:hover,
.owl-carousel .owl-nav button.owl-prev:hover {
  background: none;
}

.owl-carousel .owl-nav button.owl-next:focus,
.owl-carousel .owl-nav button.owl-prev:focus {
  outline: none;
}

.owl-theme .owl-nav [class*="owl-"] {
  background: none;
  margin: 0;
  padding: 0;
}
.owl-theme .owl-nav [class*="owl-"]:hover {
  opacity: 0.8;
  background: none;
}
</style>
