<template>
  <!-- ===== Aside Start ===== -->
  <div class="aside">
    <div class="logo">
      <a href="#"><span>A</span>VA</a>
    </div>
    <div class="nav-toggler">
      <span></span>
    </div>
    <ul class="nav">
      <li
        v-for="(item,index) in menu"
        :key="index"
      >
        <nuxt-link :to="item.link" exact-active-class="active">
          <i class="fa" :class="item.icon"></i>
          {{ item.title }}
        </nuxt-link>
      </li>
    </ul>
  </div>
  <!-- ===== Aside End ===== -->
</template>

<script>
export default {
  name: "vAside",
  data() {
    return {
      menu: [
        {
          icon: "fa-home",
          title: "Home",
          link: "/"
        },
        {
          icon: "fa-user",
          title: "About",
          link: "/about"
        },
        // {
        //   icon: "fa-list",
        //   title: "Services",
        //   link: "/services"
        // },
        {
          icon: "fa-briefcase",
          title: "Portfolio",
          link: "/portfolio"
        },
        {
          icon: "fa-comments",
          title: "Contact",
          link: "/contact"
        }
      ]
    };
  }
};
</script>
