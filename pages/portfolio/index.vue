<template>
  <div>
    <div class="main-container">
      <vAside />
      <!-- ===== Main Content Start ===== -->
      <div class="main-content">

        <!-- ===== Portfolio Section Start ===== -->
        <section class="portfolio active section" id="portfolio">
          <div class="container">
            <div class="row">
              <div class="section-title padd-15">
                <h2>Portfolio</h2>
              </div>
            </div>
            <div class="row">
              <div class="portfolio-heading padd-15">
                <h2>My Last Projects :</h2>
              </div>
            </div>
            <div class="row">
              <!-- ====== portfolio item start ====== -->
              <div
                v-for="(item,index) in info.portfolio"
                :key="index"
                class="portfolio-item padd-15"
              >
                <a :href="item.link" target="_blank">
                  <div class="portfolio-item-inner shadow-dark">
                    <div class="portfolio-img">
                      <img :src="require(`~/assets/images/portfolio/${item.img}`)" alt="">
                    </div>
                  </div>
                </a>
              </div>
            </div>
          </div>
        </section>
        <!-- ===== Portfolio Section End ===== -->

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
