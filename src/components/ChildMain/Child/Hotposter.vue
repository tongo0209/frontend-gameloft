<template>
  <div class="hotposter">
    <div class="title">
      <h1>GameLoft Game</h1>
      <div class="title__rating">
        <span>Racing / Action |</span>
        <div class="row-outer">
          <div class="container">
            <div class="star-rating">
              <input type="radio" name="rating" id="rating-5" />
              <label for="rating-5"></label>
              <input type="radio" name="rating" id="rating-4" />
              <label for="rating-4"></label>
              <input type="radio" name="rating" id="rating-3" />
              <label for="rating-3"></label>
              <input type="radio" name="rating" id="rating-2" />
              <label for="rating-2"></label>
              <input type="radio" name="rating" id="rating-1" />
              <label for="rating-1"></label>
            </div>
          </div>
        </div>
      </div>
      <div class="child">
        <div class="title__child">
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt
          accusantium, necessitatibus repellendus itaque officiis, aspernatur
          qui quae, sunt debitis maiores eius blanditiis laborum. Laudantium
          velit perferendis libero asperiores aliquam vitae.
        </div>
        <div class="icon__mxh">
          <div class="share">
            <a href="#" target="_blank"
              ><img src="../../../assets/icon/share.png" alt="logo"
            /></a>
          </div>
          <div class="mail">
            <a href="#" target="_blank"
              ><img src="../../../assets/icon/mail.png" alt="logo"
            /></a>
          </div>
          <div class="support">
            <a href="#" target="_blank"
              ><img src="../../../assets/icon/support.png" alt="logo"
            /></a>
          </div>
        </div>
      </div>
    </div>
    <div class="downloading">
      <div class="container-fluid">
        <span class="dowloading__title">Download laster version</span>
        <div class="icon">
          <a href="#" target="_blank"
            ><img
              class="downloading__child"
              src="../../../assets/icon/nintendo.png"
              alt="logo"
          /></a>
          <a href="#" target="_blank"
            ><img
              class="downloading__child"
              src="../../../assets/icon/microsoft.png"
              alt="logo"
          /></a>
          <a href="#" target="_blank"
            ><img
              class="downloading__child"
              src="../../../assets/icon/steam.png"
              alt="logo"
          /></a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.hotposter {
  width: 100%;
  height: 95vh;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  background-color: #2699fb;
  background-image: url(../../../assets/icon/icon-hotposter.png);
  background-repeat: no-repeat;
  background-size: 200px;
  background-position: 50%;
}
.title {
  padding-left: 328px;
  padding-top: 32rem;
}
.downloading {
  background-color: rgba(255, 255, 255, 0.6);
}
.child {
  display: flex;
  justify-content: space-between;
}
.icon__mxh {
  text-align: center;
  margin-right: 80px;
}
.icon__mxh .share,
.mail,
.support {
  background-color: #fff;
  border-radius: 50%;
  width: 30px;
  height: 30px;
  margin-bottom: 5px;
  border: 0;
}
.icon__mxh .share:hover,
.mail:hover,
.support:hover {
  border: 3px solid #2698fba4;
}
.container-fluid {
  display: flex;
  padding: 1rem 0;
  padding-left: 328px;
  justify-content: space-between;
  align-items: center;
}
.title h1 {
  text-transform: uppercase;
  font-size: 3rem;
  font-weight: 700;
  color: #fff;
}
.title__rating {
  display: flex;
  align-items: center;
  font-size: 20px;
  font-weight: 500;
  color: #fff;
  margin-top: 0;
  margin-bottom: 2rem;
}
.title__child {
  width: 50%;
  text-align: justify;
  font-size: 15px;
  color: #fff;
  font-weight: 500;
}
.star-rating {
  display: flex;
  justify-content: center;
  width: 100%;
  overflow: hidden;
  flex-direction: row-reverse;
  position: relative;
}
.star-rating > input {
  display: none;
}
.star-rating > label {
  margin-top: auto;
  cursor: pointer;
  width: 30px;
  height: 30px;
  background: url(https://static.vecteezy.com/system/resources/previews/001/189/080/non_2x/star-png.png)
    no-repeat center / 75%;
  transition: 0.5s;
}
.star-rating > input:not(:checked) ~ label:hover,
.star-rating > input:not(:checked) ~ label:hover ~ label {
  background: url(https://www.freepnglogos.com/uploads/star-png/star-vector-png-transparent-image-pngpix-21.png)
    no-repeat center / 75%;
}
.star-rating > input:checked ~ label,
.star-rating > input:checked ~ label ~ label {
  background: url(https://www.freepnglogos.com/uploads/star-png/star-vector-png-transparent-image-pngpix-21.png)
    no-repeat center / 75%;
}
.dowloading__title {
  color: #2699fb;
  font-weight: 700;
  width: 30%;
}
.icon {
  width: 70%;
}
.icon img {
  height: 40px;
  margin: 0 0.5rem;
  border-radius: 5px;
}
.downloading__child {
  cursor: pointer;
}
@media only screen and (max-width: 1440px) {
  .title h1 {
    font-size: 2.5rem;
  }
  .title__child {
    font-size: 14px;
  }
  .dowloading__title {
    width: 30%;
  }
}
@media only screen and (max-width: 430px) {
  .hotposter {
    height: 95vh;
    background-size: 150px;
    background-position-x: 50%;
    background-position-y: 20%;
  }
  .title {
    padding-left: 40px;
    padding-top: 25rem;
  }
  .title h1 {
    font-size: 2rem;
    width: 50%;
  }
  .title__rating {
    font-size: 12px;
    color: #fff;
    margin-bottom: 10px;
  }
  .star-rating {
    display: flex;
    justify-content: center;
    width: 100%;
    overflow: hidden;
    flex-direction: row-reverse;
    position: relative;
  }
  .star-rating > label {
    width: 18px;
    height: 18px;
  }
  .title__child {
    width: 85%;
    font-size: 12px;
    margin-bottom: 0;
    height: 50px;
    -webkit-line-clamp: 3;
    -webkit-box-orient: vertical;
    overflow: hidden;
    display: -webkit-box;
  }
  .icon__mxh {
    margin-right: 15px;
    margin-top: -2.5rem;
  }
  .container-fluid {
    display: flex;
    padding: 0;
    flex-direction: column;
    align-items: flex-start;
    padding-left: 2rem;
  }
  .icon {
    margin-bottom: 1rem;
    width: 100%;
  }
  .icon img {
    height: 50px;
    width: 180px;
    margin: 0;
    margin-top: 10px;
    margin-right: 10px;
    border-radius: 10px;
  }
  .dowloading__title {
    margin-top: 1rem;
    font-size: 25px;
    width: 100%;
  }
}
</style>