<template>
  <header>
    <div class="container">
      <nav>
        <img src="../../assets/img/light-logo.png" alt="max choach logo" />
        <ul>
          <li v-for="(link, index) in links" :key="index">
            {{ link.name }} <i class="fas fa-chevron-down"></i>
          </li>
          <li><i class="fas fa-shopping-cart"></i></li>
          <li><i class="far fa-user-circle"></i></li>
          <li>
            <div class="ricerca">
              <input class="search-bar" type="text" placeholder="Search..." />
              <i id="search" class="fas fa-search"></i>
            </div>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header",
  props: {
    links: Array,
  },
};
</script>

<style lang="scss" scoped>
header {
  color: white;
}
.container {
  height: 60px;
  background-color: #182154;
  line-height: 60px;

  nav {
    display: flex;
    align-items: center;
    justify-content: center;
    img {
      width: 150px;
      margin-right: 100px;
    }
  }
  ul {
    display: flex;
    align-items: center;
  }
  li {
    list-style: none;
    padding: 0px 15px;
    font-size: 14px;
    cursor: pointer;
  }

  .fa-chevron-down {
    font-size: 8px;
    height: 10px;
    line-height: 8px;
  }

  .ricerca {
    position: relative;
  }
  .search-bar {
    height: 35px;
    width: 150px;
    border: none;
    border-radius: 5px;
    padding: 10px;
  }
  #search {
    position: absolute;
    left: 120px;
    top: 24px;
    color: #1fad96;
  }
}
</style>
 