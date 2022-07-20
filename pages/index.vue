<template>
  <div>
    <div class="main-container">
      <vAside />
      <!-- ===== Main Content Start ===== -->
      <div class="main-content">
        <!-- ===== Home Section Start ===== -->
        <section class="home active section" id="home">
          <div class="container">
            <div class="row">
              <div class="home-info padd-15">
                <h3 class="hello">Hello, my name is <span class="name">{{ info.name }} {{ info.surname }}</span></h3>
                <h3 class="my-profession">I' m a <span class="typing">Web Developer</span></h3>
                <p>{{ info.short_description }}</p>
                <a  class="btn">Download CV</a>
              </div>
              <div class="home-img padd-15">
                <img :src="require(`~/assets/images/${info.photo}`)" alt="">
              </div>
            </div>
          </div>
        </section>
        <!-- ===== Home Section End ===== -->
      </div>
      <!-- ===== Main Content End ===== -->
    </div>
  </div>
</template>

<script>
import info from "~/data/info.json";
export default {
  data() {
    return {
      info
    };
  }
};
</script>
