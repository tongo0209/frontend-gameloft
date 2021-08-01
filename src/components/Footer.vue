<template>
  <div class="main">
    <div class="footer">
      <div class="footer__child icon__follow--min">
        <span class="icon__title">Follow us</span>
        <div class="group__share">
          <a href="#"
            ><img class="mxh" src="../assets/icon/facebook-icon.png" alt="logo"
          /></a>
          <a href="#"
            ><img class="mxh" src="../assets/icon/linkedin.png" alt="logo"
          /></a>
          <a href="#"
            ><img class="mxh" src="../assets/icon/twitter.png" alt="logo"
          /></a>
          <a href="#"
            ><img class="mxh" src="../assets/icon/youtube.png" alt="logo"
          /></a>
        </div>
      </div>
      <div class="row">
        <div class="col-9">
          <div class="footer__main">
            <div class="icon__share footer__child">
              <a href="#"
                ><img
                  class="icon__logo"
                  src="../assets/logo/logo-white.png"
                  alt="logo"
              /></a>
              <div class="footer__child icon__follow">
                <span class="icon__title">Follow us</span>
                <div class="group__share">
                  <a href="#"
                    ><img
                      class="mxh"
                      src="../assets/icon/facebook-white.png"
                      alt="logo"
                  /></a>
                  <a href="#"
                    ><img
                      class="mxh"
                      src="../assets/icon/linkedin-white.png"
                      alt="logo"
                  /></a>
                  <a href="#"
                    ><img
                      class="mxh"
                      src="../assets/icon/twitter-white.png"
                      alt="logo"
                  /></a>
                  <a href="#"
                    ><img
                      class="mxh"
                      src="../assets/icon/youtube-white.png"
                      alt="logo"
                  /></a>
                </div>
                <select name="select" id="select">
                  <option value="0">English</option>
                  <option value="1">Vietnamese</option>
                </select>
              </div>
            </div>
          </div>
        </div>
        <div class="col-3">
          <div class="visit">
            <h4>Visit</h4>
            <ul>
              <li><a href="#">Gameloft Games</a></li>
              <li><a href="#">Gameloft Careers</a></li>
              <li><a href="#">Gameloft News</a></li>
              <li><a href="#">Gameloft Forum</a></li>
              <li><a href="#">Gameloft Corporate</a></li>
              <li><a href="#">Gameloft Advertising</a></li>
              <li><a href="#">Gameloft Support</a></li>
            </ul>
          </div>
          <div class="legal">
            <h4>Legal</h4>
            <ul>
              <li><a href="#">Terms of Use</a></li>
              <li><a href="#">Privacy Policy</a></li>
              <li><a href="#">Cookies Policy</a></li>
              <li><a href="#">EULA</a></li>
              <li><a href="#">Legal Noticese</a></li>
              <li><a href="#">Event Rules</a></li>
              <li><a href="#">Business Contacts</a></li>
            </ul>
          </div>
        </div>
      </div>
    </div>
    <div class="copyright">
      <div class="content">
        ©2020 Gameloft. All rights reserved. Gameloft and the Gameloft logo are
        trademarks of Gameloft in the U.S. and/or other countries. All other
        trademarks are the property of their respective owners.
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.icon__follow--min {
  display: none;
}
.row {
  margin: 0;
}
.main {
  background-color: #2699fb;
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}
.footer {
  padding: 0;
  padding-left: 328px;
  padding-right: 200px;
}
.footer__main {
  display: flex;
  justify-content: space-between;
}
.footer__child {
  margin: 3rem 0;
}
.icon__share {
  display: flex;
  margin-top: 175px;
  flex-direction: column;
}
.icon__title {
  font-size: 20px;
  font-weight: 600;
  color: #fff;
}
.icon__logo {
  height: 60px;
}
.group__share {
  margin-top: 20px;
  margin-bottom: 20px;
}
.icon__share .mxh {
  width: 32px;
  height: 32px;
  margin-right: 1rem;
}
select {
  width: 120px;
  height: 40px;
  border: 1px solid #2699fb;
  color: #2699fb;
  padding: 0 5px;
  cursor: pointer;
}
select:focus {
  border-color: none;
  box-shadow: 0 0 1px 2px #2699fb;
  outline: none;
}
select:hover {
  color: #2699fb;
}
.visit {
  margin-top: 175px;
  color: #fff;
}
.visit h4 {
  font-size: 20px;
  font-weight: 700;
}
.visit ul {
  margin-top: 20px;
  padding-left: 0;
}
.visit ul li {
  list-style: none;
}
.visit ul li a {
  text-decoration: none;
  color: #fff;
}
.legal {
  color: #fff;
}
.legal h4 {
  font-size: 20px;
  font-weight: 700;
}
.legal ul {
  margin-top: 20px;
  padding-left: 0;
}
.legal ul li {
  list-style: none;
}
.legal ul li a {
  text-decoration: none;
  color: #fff;
}
.copyright {
  border-top: 1px solid #fff;
  display: flex;
  justify-content: center;
  text-align: center;
  height: 80px;
}
.content {
  padding-top: 1rem;
  width: 70%;
  font-weight: 300;
  color: #fff;
}

@media only screen and (max-width: 430px) {
  .main {
    height: 90vh;
  }
  .footer {
    padding: 0;
  }
  select {
    display: none;
  }
  .col-9 {
    width: 100%;
    position: relative;
  }
  .footer__child {
    text-align: center;
    width: 100%;
    margin-top: 0;
  }
  .icon__follow {
    display: none;
  }
  .col-3 {
    width: 100%;
    display: flex;
    padding: 0 20px;
  }
  .visit {
    font-weight: 600;
    width: 50%;
    font-size: 15px;
    margin-top: 0;
  }
  .visit ul li,
  .legal ul li {
    margin: 1rem 0;
  }
  .visit h4,
  .legal h4 {
    display: none;
  }
  .legal {
    width: 50%;
    font-size: 15px;
    font-weight: 600;
  }
  .icon__follow--min {
    display: block;
    background-color: rgba(255, 255, 255, 0.6);
    margin-top: 0;
    padding-top: 1rem;
    padding-bottom: 0.5rem;
  }
  .icon__follow--min .icon__title {
    color: #2699fb;
    margin-bottom: 0.5rem;
    font-size: 15px;
    padding-bottom: 0;
  }
  .icon__follow--min .mxh {
    width: 32px;
    height: 32px;
    margin-right: 1rem;
  }
  .copyright {
    border-top: 0;
    height: 80px;
  }
  .content {
    width: 100%;
    padding: 0 20px;
    text-align: center;
    font-size: 10px;
  }
}
</style>