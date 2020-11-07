<template>
  <div>
    <picture class="header-image">
      <source srcset="" media="(min-width: 800px)" />
      <img src="" alt=""
    /></picture>

    <div class="container">
      <div class="top-header-content">
        <div class="headline">
          <h2 class="top-headline">Insert your headline</h2>
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

<style scoped lang="scss"></style>
