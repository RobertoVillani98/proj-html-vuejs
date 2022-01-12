<template>
  <div class="section-top">
    <div class="text-wrapper">
      <div class="text">
        Let passion and determination be the quide along the way and develop at
        your own pace that's comfortable.
      </div>
      <div class="founder">Fannie Moreno</div>
      <div class="ceo">/Founder & CEO</div>
    </div>

    <div class="section_bottom">
      <div class="rate learners">
        <div class="num">1926</div>
        <div class="title">finished session</div>
      </div>

      <div class="rate sessions">
        <div class="num">3092+</div>
        <div class="title">enrolled learnes</div>
      </div>

      <div class="rate satisfaction">
        <div class="num">200</div>
        <div class="title">online instructors</div>
      </div>

      <div class="rate satisfaction">
        <div class="num">100%</div>
        <div class="title">satisfaction rate</div>
      </div>
    </div>
    <section class="services">
      <div class="row">
        <div class="card">
          <div class="card-title">Graphic Design</div>
          <div class="card-text">
            Have a passion for graphics and arts? Show your taltents with
            confidence and self- assertiveness.
          </div>
          <div class="card_img">
            <img src="../../assets/img/home-6-service-image-01.png" alt="" />
          </div>
        </div>
        <div class="card">
          <div class="card-title">Business Administration</div>
          <div class="card-text">
            Learners are encouraged to study the mechanism and structure of
            system administration.
          </div>
          <div class="card_img">
            <img src="../../assets/img/home-6-service-image-02.png" alt="" />
          </div>
        </div>
        <div class="card">
          <div class="card_img">
            <img src="../../assets/img/home-6-service-image-03.png" alt="" />
            <div class="card-title">Idea Discussion</div>
            <div class="card-text">
              Get teamed up with the specialist who work and teach coding for
              years at famous universities.
            </div>
          </div>
        </div>
        <div class="card">
          <div class="card_img">
            <img src="../../assets/img/home-6-service-image-04.png" alt="" />
            <div class="card-title">Web Development</div>
            <div class="card-text">
              Learns to start buiding a webpage from scratch. You decide your
              own space, course and speed.
            </div>
          </div>
        </div>
      </div>

      <div class="row-dx">
        <div class="subtitle">togheter we can create</div>
        <div class="title">Services We Can Provide For My Clients.</div>
        <div class="text">
          <i class="fas fa-check"></i>
          <span class="text-check"
            >Select & customize courses to your preferences</span
          >
        </div>
        <div class="text">
          <i class="fas fa-check"></i>
          <span class="text-check">Change the tutor and make arrangements</span>
        </div>
        <div class="text">
          <i class="fas fa-check"></i>
          <span class="text-check">Partecipate in events to join others</span>
        </div>
        <div class="text">
          <i class="fas fa-check"></i>
          <span class="text-check"
            >Get the desired certificate delivered at house</span
          >
          <Button :label="buttonLabel2" />
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import Button from "../button/Button.vue";

export default {
  components: { Button },
  name: "Section1",
  data() {
    return {
      buttonLabel2: "Get started for free",
    };
  },
};
</script>


<style lang="scss" scoped>
.section-top {
  display: flex;
  justify-content: center;
  flex-direction: column;
  align-items: center;
  padding-top: 200px;
  background-color: #ffffff;
  color: black;
  padding-bottom: 100px;
  .text-wrapper {
    text-align: center;
    display: flex;
    justify-content: center;
    flex-direction: column;
    align-items: center;
    .text {
      font-size: 25px;
      max-width: 500px;
    }
  }

  .founder {
    text-transform: uppercase;
    font-weight: bold;
    font-size: 14px;
    margin-top: 30px;
  }

  .ceo {
    color: #616865;
    font-size: 12px;
    margin-top: 20px;
  }
}

.section_bottom {
  display: flex;
  justify-content: center;
  margin-top: 100px;
  .rate {
    font-weight: bold;
    text-align: center;
    margin: 0 60px;
    .num {
      font-size: 40px;
      color: #27ab94;
    }
    .title {
      font-size: 13px;
      text-transform: uppercase;
      margin-top: 10px;
      color: #616865;
    }
  }
}
.services {
  display: flex;
  width: 100%;
  align-items: center;
  justify-content: center;
  margin-top: 60px;
  .row {
    display: grid;
    grid-template-columns: 1fr 1fr;
    margin-top: 30px;
    gap: 20px;
    .card {
      box-shadow: -1px 2px 22px 6px rgba(0, 0, 0, 0.4);
      width: 250px;
      background-color: #fff;
      overflow: hidden;
      cursor: pointer;

      .card-title {
        color: black;
        padding: 10px 20px;
      }
      .card-text {
        color: grey;
        padding: 10px 20px;
        font-size: 12px;
        line-height: 1.8;
      }

      .card_img {
        position: relative;

        img {
          width: 60%;
        }
      }
    }
  }
  .row-dx {
    display: flex;
    justify-content: center;
    flex-direction: column;
    padding: 0 150px;

    .subtitle {
      text-transform: uppercase;
      color: grey;
      font-size: 14px;
    }

    .title {
      font-size: 40px;
      max-width: 400px;
      margin: 20px 0;
      color: #27ab94;
    }
    .text {
      color: green;
      margin: 10px 0;
      font-size: 14px;

      .text-check {
        color: grey;
        margin-left: 5px;
      }
    }
  }
}
</style>