<template>
  <div>
    <picture class="header-image">
      <source srcset="" media="(min-width: 800px)" />
      <img src="" alt=""
    /></picture>

    <div class="container">
      <div class="top-header-content">
        <div class="headline">
          <h2 class="headline-top">Insert your headline</h2>
          <h2>Insert your sub-headline</h2>
        </div>
        <img src="" alt="" class="logo" />
      </div>

      <div class="bottom-header-icons">
        <div class="bottom-center">
          <div class="icon-text-container">
            <img src="" alt="" />
            <p>Text</p>
          </div>
        </div>

        <a v-scroll-to="'#scrollTo'">
          <button>Button Text</button>
        </a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Header',
}
</script>

<style scoped lang="scss">
.header-image {
  width: 100%;
  height: 100vh;
  position: relative;

  img {
    width: 100%;
    height: 100vh;
    object-fit: cover;
  }
}

button {
  background-color: transparent;
  border-radius: 50px;
  border-color: #fff;
  margin: 1rem;
  font-size: 1rem;
  padding: 0.5rem;

  @media screen and (min-width: 1251px) {
    padding: 1rem;
  }
  @media screen and (min-width: 1450px) {
    margin-left: 3rem;
  }
}

.headline {
  text-transform: uppercase;
  font-weight: bold;
  font-family: 'Bebas Neue', sans-serif;

  &-top {
    font-size: 1rem;
    @media screen and (min-width: 768px) {
      font-size: 1.7rem;
    }
  }

  h2 {
    margin: 0;
  }

  @media screen and (min-width: 768px) {
    font-size: 2rem;
    line-height: 3rem;
  }
}

.container {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  display: flex;
  justify-content: space-between;
  flex-direction: column;
  color: white;
  align-items: center;
}

.logo {
  width: 20%;
  height: auto;
}

.bottom-header-icons {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  width: 100%;
}

.bottom-center {
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  align-items: center;

  .icon-text-container {
    text-align: center;
  }

  p {
    text-align: center;
    margin: 0;
  }

  img {
    width: 15%;
    margin-top: 1rem;

    @media screen and (min-width: 768px) {
      width: 25%;
      margin-top: 0;
    }
  }

  @media screen and (min-width: 1250px) {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: flex-end;
    font-size: 1.5rem;
    width: 50%;
    p {
      width: 100%;
    }
  }
}
</style>
