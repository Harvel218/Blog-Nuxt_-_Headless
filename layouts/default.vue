<template>
  <div class="website_container">
    <header class="navigation_wraper">
      <nav class="website_navigation">
        <article class="website_logo">
          <NuxtLink to="/"> <img src="/harvel_logo.png" /></NuxtLink>
        </article>
        <SearchArticle />
      </nav>
    </header>

    <Nuxt />
  </div>
</template>

<style lang="scss">
html {
  font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Roboto, 'Helvetica Neue', Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
}

a,
p,
h1,
h2,
h3,
h4,
h5,
div,
article,
section,
main,
footer,
nav,
span {
  text-decoration: none;
  color: $main_font_color;
}

ul {
  list-style: none;
  padding: 0;
  width: 100%;
}

body {
  margin: 0;
  padding: 0;
  min-width: 100vw;
  width: 100vw;
  max-width: 100vw;
  min-height: 100vh;
  height: auto;
  overflow-x: hidden;
  background-color: $page_bg;

  & .website_container {
    min-width: 320px;
    width: 100%;
    max-width: 820px;
    height: 120vh;
    margin: 0 auto;
    position: relative;

    & .navigation_wraper {
      width: 100%;
      height: 90px;
      position: relative;

      & .website_navigation {
        width: 100%;
        height: 90px;
        max-width: 820px;
        display: flex;
        justify-content: space-between;
        align-items: flex-end;
        position: fixed;
        top: 0;
        background-color: $main_page_color;
        padding-bottom: 15px;
        border-radius: 0 0 5px 5px;

        & .website_logo {
          display: flex;
          justify-content: center;
          align-items: flex-end;
          width: 75px;
          margin-left: 15px;
          padding-left: 5px;
          padding-right: 5px;
          border-radius: 0 0 5px 5px;
          background-color: $main_page_color;
          height: 100%;

          & img {
            width: 100%;
            height: auto;
          }
        }
      }
    }
  }
}
</style>
