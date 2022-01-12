<template>
  <div class="blog">
    <h3>Enjoy reading on maxcoach</h3>
    <h2>Latest on <span>Our Blogs</span></h2>
    <div class="row">
      <div class="card">
        <img src="../../assets/img/artist-blog-03-480x325.jpeg" alt="" />
        <div class="card-text">
          <div class="artist">
            <p>artist</p>
          </div>
          <div class="desc">Brush Strokes Eneraize Tress in Paintings</div>

          <div class="lessons">
            <i class="far fa-calendar"></i>
            <p>May 15, 2020</p>
            <i class="far fa-eye"></i>
            <p>688 views</p>
          </div>
        </div>
      </div>

      <div class="card">
        <img src="../../assets/img/artist-blog-01-480x325.jpg" alt="" />
        <div class="card-text">
          <div class="artist">
            <p>artist</p>
          </div>
          <div class="desc">
            Pocket-Sized Notebooks Hold Miniature Paintings
          </div>
          <div class="lessons">
            <i class="far fa-calendar"></i>

            <p>May 15, 2020</p>
            <i class="far fa-eye"></i>
            <p>602 views</p>
          </div>
        </div>
      </div>

      <div class="card">
        <img src="../../assets/img/artist-blog-02-480x325.jpg" alt="" />
        <div class="card-text">
          <div class="artist">
            <p>artist</p>
          </div>
          <div class="desc">Connection Between Self-Portraits and Identity</div>
          <div class="lessons">
            <i class="far fa-calendar"></i>
            <p>May 15, 2020</p>
            <i class="far fa-eye"></i>

            <p>397 views</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Section4",
};
</script>

<style lang="scss" scoped>
.blog {
  background-color: #f8f8f8;
  display: flex;
  align-items: center;
  flex-direction: column;
  padding: 80px 0;

  h3 {
    text-transform: uppercase;
    color: grey;
    font-size: 13px;
    font-weight: 200;
  }
  h2 {
    font-size: 40px;
    margin: 20px 0;
    font-weight: 400;

    span {
      color: #27ab94;
    }
  }

  .row {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    margin: 40px 500px;
    gap: 20px;
  }

  .card {
    display: flex;
    flex-wrap: wrap;
  }
  img {
    width: 100%;
    height: 200px;
    object-fit: cover;
    border-radius: 5px;
  }

  .card-text {
    margin-top: 20px;
    .artist {
      font-size: 14px;
      color: grey;
      text-transform: uppercase;
    }

    .desc {
      padding: 10px 0;
      line-height: 1.6;
    }
  }
  .lessons {
    display: flex;
    flex-direction: row;
    color: grey;

    p {
      margin-right: 20px;
      margin-left: 5px;
      font-size: 11px;
      font-weight: 200;
    }
  }
}
</style>