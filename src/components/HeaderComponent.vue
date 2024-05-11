<template>
  <div class="navigation">
    <img src="/logo.png" alt="logo" class="logo" /><img />
    <ul class="menu" :class="{ aktif: isMenuActive }">
      <li><a href="#home" :class="{ aktif: isMenuActive }">Home</a></li>
      <li><a href="#about">About us</a></li>
      <li><a href="#service">Our Service</a></li>
      <li><a href="#company">Company Values</a></li>
      <li><a href="#contact">Contact Us</a></li>
    </ul>
    <div class="button" @click="toggleMenu">&#9776;</div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      isMenuActive: false,
    };
  },
  methods: {
    toggleMenu() {
      this.isMenuActive = !this.isMenuActive;
    },
  },
};
</script>

<style scoped>
.logo {
  width: 120px;
}
.navigation {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.button {
  display: none;
  color: black;
  font-size: 14pt;
}

.button:hover {
  cursor: pointer;
}

.menu {
  margin: 0;
  display: flex;
  list-style: none;
  font-size: 12pt;
}

.menu li {
  padding-left: 0;
}

.menu li a {
  padding: 10px;
  color: black;
  text-decoration: none;
  display: inline-block;
  padding: 12px;
}

.menu li a:hover {
  color: #110f5e;
  background-color: #fddc58;
  border-radius: 12px;
}

@media screen and (max-width: 768px) {
  .menu {
    display: none;
  }

  .menu.aktif {
    display: block;
    position: absolute;
    top: 50px;
    background: rgba(247, 247, 247, 1);
    right: 0;
    left: 0;
    text-align: center;
  }

  .menu.aktif li a {
    display: block;
  }
  .menu.aktif li a {
    border-radius: 0px;
  }

  .button {
    display: block;
  }
}
</style>
