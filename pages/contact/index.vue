<template>
  <div>
    <div class="main-container">
      <vAside />
      <!-- ===== Main Content Start ===== -->
      <div class="main-content">

        <!-- ===== Contact Section Start ===== -->
        <section class="contact active section" id="contact">
          <div class="container">
            <div class="row">
              <div class="section-title padd-15">
                <h2>Contact Me</h2>
              </div>
            </div>
            <h3 class="contact-title padd-15">Have You Any Questions ?</h3>
            <h4 class="contact-sub-title padd-15">I'M AT YOUR SERVICES</h4>
            <div class="row">
              <!-- ===== Contact info item start ====== -->
              <div class="contact-info-item padd-15">
                <div class="icon"><i class="fa fa-phone"></i></div>
                <h4>Call Us On</h4>
                <p>{{info.phone}}</p>
              </div>
              <!-- ===== Contact info item end ====== -->
              <!-- ===== Contact info item start ====== -->
              <div class="contact-info-item padd-15">
                <div class="icon"><i class="fa fa-map-marker-alt"></i></div>
                <h4>Office</h4>
                <p>{{ info.country }}</p>
              </div>
              <!-- ===== Contact info item end ====== -->
              <!-- ===== Contact info item start ====== -->
              <div class="contact-info-item padd-15">
                <div class="icon"><i class="fa fa-envelope"></i></div>
                <h4>Email</h4>
                <p>{{ info.email }}</p>
              </div>
              <!-- ===== Contact info item end ====== -->
              <!-- ===== Contact info item start ====== -->
              <div class="contact-info-item padd-15">
                <div class="icon"><i class="fa fa-globe-europe"></i></div>
                <h4>Website</h4>
                <p>{{ info.website }}</p>
              </div>
              <!-- ===== Contact info item end ====== -->
            </div>
<!--            <h3 class="contact-title padd-15">SEND ME AN EMAIL</h3>-->
<!--            <h4 class="contact-sub-title padd-15">I'M VERY RESPOSIVE TO MESSAGES</h4>-->
<!--            &lt;!&ndash; ====== Contact Form ====== &ndash;&gt;-->
<!--            <div class="row">-->
<!--              <div class="contact-form padd-15">-->
<!--                <div class="row">-->
<!--                  <div class="form-item col-6 padd-15">-->
<!--                    <div class="form-group">-->
<!--                      <input type="text" class="form-control" placeholder="Name">-->
<!--                    </div>-->
<!--                  </div>-->
<!--                  <div class="form-item col-6 padd-15">-->
<!--                    <div class="form-group">-->
<!--                      <input type="email" class="form-control" placeholder="Email">-->
<!--                    </div>-->
<!--                  </div>-->
<!--                </div>-->
<!--                <div class="row">-->
<!--                  <div class="form-item col-12 padd-15">-->
<!--                    <div class="form-group">-->
<!--                      <input type="text" class="form-control" placeholder="Subject">-->
<!--                    </div>-->
<!--                  </div>-->
<!--                </div>-->
<!--                <div class="row">-->
<!--                  <div class="form-item col-12 padd-15">-->
<!--                    <div class="form-group">-->
<!--                      <textarea name="" class="form-control" id="" placeholder="Message"></textarea>-->
<!--                    </div>-->
<!--                  </div>-->
<!--                </div>-->
<!--                <div class="row">-->
<!--                  <div class="form-item col-12 padd-15">-->
<!--                    <button type="submit" class="btn">Send Message</button>-->
<!--                  </div>-->
<!--                </div>-->
<!--              </div>-->
<!--            </div>-->
          </div>
        </section>
        <!-- ===== Contact Section End ===== -->
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
