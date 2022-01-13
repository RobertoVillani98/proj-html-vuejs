<template>
  <div class="helps">
    <div class="help">
      <div class="help-subtitle">wanna transform your life</div>
      <div class="help-title">Glad to <span>Help You</span> Learn</div>
    </div>

    <div class="row">
      <div class="card">
        <i class="far fa-flag"></i>
        <div class="card-text">
          <div class="title">
            <p>Idea Discussion</p>
          </div>
          <div class="desc">
            <p>
              Get teamed up with the specialists who work and teach coding for
              years at famous universities.
            </p>
          </div>
        </div>
      </div>

      <div class="card">
        <i class="fas fa-cog"></i>
        <div class="card-text">
          <div class="title">
            <p>Web Development</p>
          </div>
          <div class="desc">
            <p>
              Learn to start building a webpages from scratch. You decide your
              own pace, cuorse and speed.
            </p>
          </div>
        </div>
      </div>

      <div class="card">
        <i class="far fa-life-ring"></i>
        <div class="card-text">
          <div class="title">
            <p>System Administration</p>
          </div>
          <div class="desc">
            <p>
              Learners are encouraged to study the mechanism and structure of
              system administration.
            </p>
          </div>
        </div>
      </div>

      <div class="card">
        <i class="fas fa-desktop"></i>
        <div class="card-text">
          <div class="title">
            <p>Graphic Design</p>
          </div>
          <div class="desc">
            <p>
              Have a passion for graphics and arts? Show your talents with
              confidence and self-asssertiveness.
            </p>
          </div>
        </div>
      </div>

      <div class="image">
        <img src="../../assets/img/home-6-services-image-1024x411.png" alt="" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Help",
};
</script>

<style lang="scss" scoped>
.helps {
  background: linear-gradient(
    to bottom,
    #ffffff,
    #f8f8f8,
    #f1f1f1,
    #eaeaea,
    #e3e3e3
  );

  display: flex;
  align-items: center;
  flex-direction: column;

  .help {
    text-align: center;
    padding: 80px 0;

    &-subtitle {
      text-transform: uppercase;
      color: grey;
      font-size: 13px;
      font-weight: 200;
    }

    &-title {
      font-size: 40px;
      margin: 20px 0;
      font-weight: 400;

      span {
        color: #27ab94;
      }
    }
  }
  .row {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr 1fr;
    margin: 0 250px;
    gap: 10px;
  }

  .card {
    display: flex;
    flex-wrap: wrap;
  }

  .fa-flag {
    font-size: 50px;
  }

  .fa-cog {
    font-size: 50px;
  }

  .fa-life-ring {
    font-size: 50px;
  }

  .fa-desktop {
    font-size: 50px;
  }

  .card-text {
    margin: 50px 0;

    .title {
      font-size: 18px;
    }

    .desc {
      font-size: 14px;
      color: grey;
      margin: 10px 0;
      line-height: 1.6;
      font-weight: 200;
      width: 80%;
    }
  }

  .image img {
    width: 250%;
    margin: -20px 110px;
  }
}
</style>