<template>
  <div class="why">
    <h2>Whyc People Talk About <span>MaxCoach</span>?</h2>
    <div class="row">
      <div class="card">
        <img
          class="testimonial"
          src="../../assets/img/testimonial-avata-02.jpg"
          alt=""
        />
        <div class="card-text">
          <p>
            I am free to learn at my own pace, follow my own schedule and choose
            the subject I like. Great study portal for people like me.
          </p>
          <h4>mina Hollace</h4>
          <h5>/ Freelancer</h5>
        </div>
      </div>
    </div>
    <div class="section_bottom">
      <div class="logo-img">
        <img
          class="logo"
          src="../../assets/img/client-logo-colored-01.png"
          alt=""
        />
        <img
          class="logo"
          src="../../assets/img/client-logo-colored-02.png"
          alt=""
        />
        <img
          class="logo"
          src="../../assets/img/client-logo-colored-03.png"
          alt=""
        />
        <img
          class="logo"
          src="../../assets/img/client-logo-colored-04.png"
          alt=""
        />
        <img
          class="logo"
          src="../../assets/img/client-logo-colored-05.png"
          alt=""
        />
        <img
          class="logo"
          src="../../assets/img/client-logo-colored-06.png"
          alt=""
        />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Section3",
};
</script>

<style lang="scss" scoped>
.why {
  height: 500px;
  display: flex;
  align-items: center;
  flex-direction: column;
  padding: 100px 0;

  h2 {
    font-size: 36px;
    font-weight: 400;
    margin-bottom: 40px;

    span {
      color: #27ab94;
    }
  }

  .row {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
  }

  .card {
    display: flex;
    justify-content: center;
  }

  .testimonial {
    margin-right: 50px;
    margin-top: 50px;
    width: 150px;
    height: 150px;
    border-radius: 50%;
    object-fit: cover;
  }

  .card-text {
    display: flex;
    flex-direction: column;
    justify-content: center;
    width: 50%;
    height: 100%;
    max-width: 1000px;
    padding: 50px;

    p {
      font-size: 26px;
      line-height: 1.4;
      color: grey;
      font-weight: 300;
    }

    h4 {
      margin-top: 20px;
      text-transform: uppercase;
      font-size: 12px;
      font-weight: 500;
    }

    h5 {
      color: grey;
      margin-top: 10px;
      font-weight: 200;
      font-size: 10px;
    }
  }
}

.section_bottom {
  display: flex;
  justify-content: center;
  width: 100%;
  margin-top: 30px;
  padding-bottom: 100px;

  .logo-img {
    display: flex;
    justify-content: space-between;
    width: 45%;
  }

  .logo {
    width: 70px;
    object-fit: contain;
  }
}
</style>