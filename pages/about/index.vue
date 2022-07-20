<template>
  <div>
    <div class="main-container">
      <vAside />
      <!-- ===== Main Content Start ===== -->
      <div class="main-content">

        <!-- ===== About Section Start ===== -->
        <section class="about active section" id="about">
          <div class="container">
            <div class="row">
              <div class="section-title padd-15">
                <h2>About Me</h2>
              </div>
            </div>
            <div class="row">
              <div class="about-content padd-15">
                <div class="row">
                  <div class="about-text padd-15">
                    <h3>I'm {{ info.name }} {{ info.surname }} and <span>Web Developer</span></h3>
                    <p> {{ info.description }} </p>
                  </div>
                </div>
                <div class="row">
                  <div class="personal-info padd-15">
                    <div class="row">
                      <div class="info-item padd-15">
                        <p>Birthday : <span>{{ info.birthday }}</span></p>
                      </div>
                      <div class="info-item padd-15">
                        <p>Age : <span>{{ info.age }}</span></p>
                      </div>
                      <div class="info-item padd-15">
                        <p>Website : <span>{{ info.website }}</span></p>
                      </div>
                      <div class="info-item padd-15">
                        <p>Email : <a :href="`mailto:${info.email}`"><span>{{ info.email }}</span></a></p>
                      </div>
                      <div class="info-item padd-15">
                        <p>Degree : <span>{{ info.degree }}</span></p>
                      </div>
                      <div class="info-item padd-15">
                        <p>Phone : <a :href="`tel:${info.phone}`"> <span>{{ info.phone }}</span> </a></p>
                      </div>
                      <div class="info-item padd-15">
                        <p>Country : <span>{{ info.country }}</span></p>
                      </div>
                      <div class="info-item padd-15">
                        <p>City : <span>{{ info.city }}</span></p>
                      </div>
                      <div class="info-item padd-15">
                        <p>Freelnace : <span>{{ info.freelnace }}</span></p>
                      </div>
                    </div>
                    <div class="row">
                      <div class="buttons padd-15">
                        <nuxt-link to="/contact" data-section-index="1" class="btn hire-me">Hire Me</nuxt-link>
                      </div>
                    </div>
                  </div>
                  <div class="skills padd-15">
                    <div class="row">
                      <div
                        v-for="(item,index) in info.skills"
                        :key="index"
                        class="skill-item padd-15"
                      >
                        <h5>{{ item.name }}</h5>
                        <div class="progress">
                          <div class="progress-in" :style="`width: ${item.percent}%;`"></div>
                          <div class="skill-percent">{{ item.percent }}%</div>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
                <div class="row">
                  <div class="education padd-15">
                    <h3 class="title">Education</h3>
                    <div class="row">
                      <div class="timeline-box padd-15">
                        <div class="timeline shadow-dark">
                          <!-- ===== timeline item ===== -->
                          <div
                            v-for="(item,index) in info.education"
                            :key="index"
                            class="timeline-item"
                          >
                            <div class="circle-dot"></div>
                            <h3 class="timeline-date">
                              <i class="fa fa-calendar"></i> {{ item.date }}
                            </h3>
                            <h4 class="timeline-title">{{ item.title }}</h4>
                            <p class="timeline-text">{{ item.description }}</p>
                          </div>
                          <!-- ===== timeline item ===== -->
                        </div>
                      </div>
                    </div>
                  </div>
                  <div class="experience padd-15">
                    <h3 class="title">Experience</h3>
                    <div class="row">
                      <div class="timeline-box padd-15">
                        <div class="timeline shadow-dark">
                          <!-- ===== timeline item ===== -->
                          <div
                            v-for="(item,index) in info.experience"
                            :key="index"
                            class="timeline-item"
                          >
                            <div class="circle-dot"></div>
                            <h3 class="timeline-date">
                              <i class="fa fa-calendar"></i> {{ item.date }}
                            </h3>
                            <h4 class="timeline-title">{{ item.title }}</h4>
                            <p class="timeline-text">{{ item.description }}</p>
                          </div>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </section>
        <!-- ===== About Section End ===== -->
      </div>
      <!-- ===== Main Content End ===== -->
    </div>
  </div>
</template>

<script>
import info from "@/data/info.json";

export default {
  data() {
    return {
      info
    };
  }
};
</script>
