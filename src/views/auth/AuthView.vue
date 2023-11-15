<template>
  <div class="wrapper">
    <div class="form">
      <div class="form-logo">
        <img
          src="https://www.sdu.dk/-/media/files/nyheder/logoer/sdu_white_rgb-png.png"
          alt="logo"
          width="120"
        />
      </div>
      <div class="form-fields">
        <input type="text" placeholder="Введите имя" />
        <input type="email" placeholder="Введите почту" />
      </div>
    </div>
  </div>
</template>

<script lang="ts" setup></script>

<style scoped lang="scss">
.wrapper {
  width: 100vw;
  height: 100vh;
  position: relative;
  background-image: url("../../../public/images/auth-desktop-background.jpg");
  //background-image: url("https://cdn.fakty.com.ua/wp-content/uploads/2018/09/28/dreamstime_l_93541823-e1578142834928-scaled.jpg");
  //background-image: url("https://starwalk.space/gallery/images/what-is-space/1920x1080.jpg");
  background-size: cover;
  background-repeat: no-repeat;
  @media (max-width: 768px) {
    background-image: url("../../../public/images/auth-mobile-background.jpg");
  }
}

.form {
  width: 400px;
  height: 300px;
  border-radius: 16px;
  background-color: rgba(255, 255, 255, 0.05);
  box-shadow: 0 0 1px rgba(255, 255, 255, 1);
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  box-sizing: border-box;
  padding: 16px;
  @media (max-width: 768px) {
    max-width: 90vw;
    width: 100%;
    height: 300px;
    top: 35%;
  }

  &-logo {
    text-align: center;
    margin-bottom: 24px;
  }

  &-fields {
    display: flex;
    flex-direction: column;
    gap: 16px;

    input {
      height: 48px;
      outline: none;
      border: none;
      background: #fff;
      border-radius: 4px;
      padding: 0 16px;
    }
  }
}
</style>
