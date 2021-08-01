<template>
  <div class="main">
    <div class="row">
      <div class="col-6 col__logo">
        <img src="../../assets/icon/icon-minion.png" alt="" />
      </div>
      <div class="col-6 col__register">
        <div class="title">Stay in the Know!</div>
        <div class="title__child">Don't get left behind!</div>
        <input
          type="text"
          class="form-control form__input"
          id="name"
          placeholder="Name"
        />
        <input
          type="email"
          class="form-control form__input"
          id="email"
          placeholder="Email"
        />
        <select name="select" id="select">
          <option selected>Country</option>
          <option value="1">Vietnamese</option>
        </select>
        <select name="select" id="select">
          <option selected>Flatform</option>
          <option value="1">Select</option>
        </select>
        <div class="form-check">
          <input
            class="form-check-input"
            type="checkbox"
            value=""
            id="flexCheckDefault"
          />
          <label class="form-check-label" for="flexCheckDefault">
            By signing up, I confirm that I am 13 years old or older. I agree to
            the Gameloft Terms and Conditions
          </label>
        </div>
        <div class="form-check">
          <input
            class="form-check-input"
            type="checkbox"
            value=""
            id="flexCheckDefault"
          />
          <label class="form-check-label" for="flexCheckDefault">
            I agree to receive promotional offers relating to all Gameloft games
            and services.
          </label>
        </div>
        <div class="btn-group" role="group">
          <button type="button" class="btn btn-outline-primary">Button</button>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {};
</script>

<style scoped>
.main {
  height: 100vh;
  background-color: #d8edff;
}
.row {
  padding-left: 328px;
  padding-right: 100px;
  padding-top: 200px;
  display: flex;
}
.title {
  font-size: 28px;
  font-weight: 700;
  color: #2699fb;
}
.title__child {
  font-size: 15px;
  color: #2699fb;
}
.form__input {
  margin: 1rem 0;
  border: 1px solid #2699fb;
  color: #2699fb;
  background-color: transparent;
}
.form__input::placeholder {
  color: #2699fb;
}
select {
  width: 100%;
  margin: 0.5rem 0;
  height: 40px;
  border: 1px solid #2699fb;
  color: #2699fb;
  padding: 0 5px;
  border-radius: 5px;
  cursor: pointer;
  background-color: transparent;
}
select:focus {
  border-color: none;
  box-shadow: 0;
  outline: none;
}
.form-check {
  margin: 1rem 0;
  color: #2699fb;
  font-size: 15px;
}
.col__register {
  width: 40%;
}
.form-check input {
  border: 1px solid #2699fb;
  border-radius: 0;
}
.btn-group {
  display: flex;
  width: 35%;
  margin: 0 auto;
}
.btn-outline-primary {
  border: 1px solid #2699fb;
  color: #2699fb;
  padding: 0.5rem;
}
.btn-outline-primary:hover {
  background-color: #2699fb;
  color: #fff;
}
@media only screen and (max-width: 1440px) {
}
@media only screen and (max-width: 430px) {
  .row {
    padding: 0;
    padding-top: 120px;
    display: flex;
  }
  .col__logo {
    display: none;
  }
  .col__register {
    width: 100%;
    display: flex;
    flex-direction: column;
    padding: 0 60px;
  }
  .form-check {
    font-size: 12px;
  }
  .btn-outline-primary {
    padding: 0.25rem;
  }
}
</style>