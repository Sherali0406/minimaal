<template>
  <div class="navbar">
    <div class="logo">
      <img class="image" :src="image1" alt="Logo" />
      <h1 class="minimal">Minimal</h1>
    </div>
    <div class="texts">
      <h2>process</h2>
      <h2>projects</h2>
      <h2>team</h2>
      <h2>contact</h2>
    </div>
  </div>
</template>

<script setup>
import image1 from "../../public/logo.png";
</script>

<style lang="scss" scoped>
.navbar {
  display: flex;
  flex-direction: row;
  width: 100%;
  height: 106px;
  justify-content: center;
  gap: 400px;
  .logo {
    display: flex;
    flex-direction: row;
    gap: 50px;

    .image {
      width: 65px;
      height: 70px;
      flex-shrink: 0;
      padding-top: 5px;
    }
    .minimal {
      color: #333;
      font-family: Oswald;
      font-size: 22px;
      font-style: normal;
      font-weight: 400;
      line-height: 38px;
      text-transform: uppercase;
      width: 72px;
    }
  }
  .texts {
    width: auto;
    display: flex;
    height: 45px;
    padding: 23px 0px 0px 34px;
    justify-content: flex-end;
    align-items: flex-start;
    gap: 34px;
    h2 {
      color: #404040;
      font-family: Montserrat;
      font-size: 12px;
      font-style: normal;
      font-weight: 400;
      line-height: 20px;
      text-transform: uppercase;
      &:hover {
        transition: all 0.3s linear;
        cursor: pointer;
      }
    }
  }
}
@media screen and (max-width: 960px) {
  .navbar {
    display: flex;
    flex-direction: row;
    width: 100%;
    height: 106px;
    justify-content: center;
    gap: 20px;
  }
}

@media screen and (max-width: 560px) {
  .navbar {
    gap: 10px;
    .logo {
      gap: 10px;

      .image {
        width: 50px;
        height: 50px;
      }
      .minimal {
        font-size: 18px;
      }
    }
    .texts {
      gap: 15px;
      h2 {
        font-size: 10px;
        &:hover {
          transition: all 0.3s linear;
          cursor: pointer;
        }
      }
    }
  }
}

@media screen and (max-width: 460px) {
  .navbar {
    gap: 5px;
    .logo {
      gap: 5px;

      .image {
        width: 40px;
        height: 40px;
      }
      .minimal {
        font-size: 15px;
      }
    }
    .texts {
      gap: 10px;
      h2 {
        font-size: 8px;
        &:hover {
          transition: all 0.3s linear;
          cursor: pointer;
        }
      }
    }
  }
}
</style>
