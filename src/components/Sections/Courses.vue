<template>
  <div class="courses">
    <h3>Chose a course to get started</h3>
    <h2>Latest Featured <span>Courses</span></h2>
    <div class="row">
      <div class="card">
        <img src="../../assets/img/course-02-480x298.jpg" alt="" />
        <div class="card-text">
          <div class="price">
            <p>$40<span>.00</span></p>
          </div>
          <div class="desc">Learning to write as a Professional Author</div>

          <div class="lessons">
            <i class="fas fa-newspaper"></i>
            <p>20 lessons</p>
            <i class="far fa-user"></i>
            <p>50 Students</p>
          </div>
        </div>
      </div>

      <div class="card">
        <img src="../../assets/img/stock-full-hd-03-480x298.jpg" alt="" />
        <div class="card-text">
          <div class="price">
            <p>Free</p>
          </div>
          <div class="desc">Customer-centric Info-Tech Strategies</div>

          <div class="lessons">
            <i class="fas fa-newspaper"></i>
            <p>24 lessons</p>
            <i class="far fa-user"></i>
            <p>769 Students</p>
          </div>
        </div>
      </div>

      <div class="card">
        <img src="../../assets/img/stock-full-hd-04-480x298.jpg" alt="" />
        <div class="card-text">
          <div class="price">
            <p>$19<span>.00</span></p>
          </div>
          <div class="desc">Open Programming Courses for Everyone: Python</div>

          <div class="lessons">
            <i class="fas fa-newspaper"></i>
            <p>17 lessons</p>
            <i class="far fa-user"></i>
            <p>62 Students</p>
          </div>
        </div>
      </div>

      <div class="card">
        <img src="../../assets/img/stock-full-hd-06-480x298.jpg" alt="" />
        <div class="card-text">
          <div class="price">
            <p>$26<span>.00</span></p>
          </div>
          <div class="desc">Academic Listening and Note-taking</div>

          <div class="lessons">
            <i class="fas fa-newspaper"></i>
            <p>14 lessons</p>
            <i class="far fa-user"></i>
            <p>67 Students</p>
          </div>
        </div>
      </div>

      <div class="card">
        <img
          src="../../assets/img/course-featured-image-01-480x298.jpg"
          alt=""
        />
        <div class="card-text">
          <div class="price">
            <p>$39<span>.00</span></p>
          </div>
          <div class="desc">Master jQeury in a Short Period of Time</div>
          <div class="lessons">
            <i class="fas fa-newspaper"></i>
            <p>6 lessons</p>
            <i class="far fa-user"></i>
            <p>51 Students</p>
          </div>
        </div>
      </div>

      <div class="card">
        <img src="../../assets/img/stock-full-hd-05-480x298.jpg" alt="" />
        <div class="card-text">
          <div class="price">
            <p>$59<span>.00</span></p>
          </div>
          <div class="desc">Introduction to Javascript for Beginners</div>

          <div class="lessons">
            <i class="fas fa-newspaper"></i>
            <p>14 lessons</p>
            <i class="far fa-user"></i>
            <p>76 Students</p>
          </div>
        </div>
      </div>
    </div>
    <Button :label="buttonLabel3" />
  </div>
</template>

<script>
import Button from "../button/Button.vue";
export default {
  components: { Button },
  name: "Section2",
  data() {
    return {
      buttonLabel3: "View all courses →",
    };
  },
};
</script>

<style lang="scss" scoped>
.courses {
  display: flex;
  align-items: center;
  flex-direction: column;
  padding: 100px 0;
  background-color: #f5f7fa;

  h3 {
    text-transform: uppercase;
    color: grey;
    font-size: 13px;
    font-weight: 200;
  }
  h2 {
    font-size: 40px;
    margin: 20px 0;
    font-weight: 600;

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
    flex-wrap: wrap;
    justify-content: center;
    width: 35%;
  }
  img {
    margin: 30px 20px;
    width: 120px;
    height: 120px;
    border-radius: 50%;
    object-fit: cover;
  }

  .card-text {
    display: flex;
    flex-direction: column;
    justify-content: center;
    width: 50%;

    .price {
      font-size: 18px;
      color: #27ab94;
      font-weight: bold;

      span {
        font-size: 12px;
      }
    }

    .desc {
      padding: 10px 0;
      cursor: pointer;
      &:hover {
        color: #27ab94;
      }
    }

    .lessons {
      display: flex;
      flex-direction: row;
      color: grey;

      p {
        margin-right: 20px;
        margin-left: 5px;
        font-size: 12px;
      }
    }
  }
}
</style>