<template>
  <div id="app" class="is-max-desktop">
    <TopBar />
    <Navigation />
    <Carousel />
    <Sidebar />
    <ShipingInfo />
    <Gallery />
    <router-view />
  </div>
</template>
<script>
import Navigation from "@/components/Navigation";
import Sidebar from "@/components/Sidebar";
import TopBar from "@/components/TopBar";
import Carousel from "@/components/Carousel";
import ShipingInfo from "@/components/ShipingInfo";
import Gallery from "@/components/Gallery";

export default {
  components: {
    Navigation,
    Sidebar,
    TopBar,
    Carousel,
    ShipingInfo,
    Gallery,
  },
};
</script>
<style >
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
  color: #1e7fc0;
}
.navbar-burger {
  position: absolute !important;
  right: 0 !important;
}
.navbar-burger:hover span {
  color: orange;
}
.navbar-burger:hover {
  background-color: transparent !important;
}
.navbar-burger span {
  height: 2px !important;
  width: 20px !important;
}
@media screen and (min-width: 1024px) {
  .navbar-burger {
    display: block !important;
  }
}
@media screen and (max-width: 1023px) {
  .navbar-menu {
    display: none !important;
  }
}
</style>

