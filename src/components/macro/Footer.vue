<template>
  <footer>
    <div class="container_small">
      <nav class="footer_nav">
        <ul>
          <li>
            <a href="#">{{ contacts.title }}</a>
          </li>
          <li>
            <a href="#">{{ contacts.address }}</a>
          </li>
          <li>
            <a href="#">{{ contacts.tel }}</a>
          </li>
          <li>
            <a href="#">{{ contacts.mail }}</a>
          </li>
          <li id="social_links">
            <ul>
              <li>
                <a href="https://it-it.facebook.com/" target="“blank”"
                  ><i class="fab fa-facebook-square"></i
                ></a>
              </li>
              <li>
                <a href="https://www.twitter.com" target="“blank”"
                  ><i class="fab fa-twitter"></i
                ></a>
              </li>
              <li>
                <a href="https://www.instagram.com" target="“blank”"
                  ><i class="fab fa-instagram"></i
                ></a>
              </li>
              <li>
                <a href="https://it.linkedin.com/" target="“blank”"
                  ><i class="fab fa-linkedin"></i
                ></a>
              </li>
            </ul>
          </li>
        </ul>

        <ul
          v-for="(link, i) in links"
          :key="i"
          :class="{ contacts: link.title == 'Contacts' }"
        >
          <li>
            <a href="#">{{ link.title }}</a>
          </li>
          <li v-for="(el, i) in link.elements" :key="i">
            <a :href="el.link">{{ el.name }}</a>
          </li>
        </ul>
      </nav>

      <div class="rights">©2020 Maxcoach. All Rights Reserved</div>
    </div>

    <div class="btn btn_up">
      <a href="#"><i class="fas fa-long-arrow-alt-up"></i></a>
    </div>
  </footer>
</template>

<script>
export default {
  name: "Footer",
  props: {
    links: Array,
    contacts: Object,
  },
};
</script>


<style lang="scss" scoped>
footer {
  background-color: #f1efef;
  padding: 50px 0;
  position: relative;
  .footer_nav {
    display: flex;
    justify-content: space-around;
    margin: 0 250px;
    ul {
      list-style: none;
      &:first-of-type {
        flex-grow: 0.5;
      }
      li:not(:first-child) {
        margin: 10px 0;
        a {
          font-size: 12px;
          color: #616865;
          text-decoration: none;
        }
      }
      li:first-child:not(#social_links li) {
        a {
          font-size: 13px;
          font-weight: bold;
          color: black;
          text-decoration: none;
        }
      }
      &.contacts {
        li:first-child {
          opacity: 0;
        }
      }
      #social_links {
        ul {
          margin: 15px 0;
          li {
            display: inline-block;
            margin-right: 20px;
            .fa-facebook-square {
              font-size: 20px;
              color: #616865;
            }

            .fa-twitter {
              font-size: 20px;
              color: #616865;
            }

            .fa-instagram {
              font-size: 20px;
              color: #616865;
            }

            .fa-linkedin {
              font-size: 20px;
              color: #616865;
            }
          }
        }
      }
    }
  }

  .rights {
    font-size: 12px;
    text-align: center;
    color: #616865;
    margin-top: 30px;
  }
  .btn_up {
    width: 40px;
    height: 40px;
    line-height: 40px;
    text-align: center;
    background-color: #27ab94;
    border-radius: 50%;
    cursor: pointer;
    position: absolute;
    right: 40px;
    bottom: 40px;
    a {
      width: 40px;
      height: 40px;
      color: white;
      display: inline-block;
    }
  }
}
</style>