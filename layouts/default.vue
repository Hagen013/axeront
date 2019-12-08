<template>
  <div class="page">
    <div class="page-body">
      <Header/>
      <div class="main">
        <nuxt/>
      </div>
      <Footer/>
    </div>
    <Sidebar/>
  </div>
</template>

<script>
import Header from '@/components/Header'
import Footer from '@/components/Footer'
import Sidebar from '@/components/Sidebar'

export default {
  components: {
    Header,
    Footer,
    Sidebar
  }
}
</script>

<style rel="stylesheet/scss" lang="scss">

@import "node_modules/sass-mq/mq";

@import '~assets/scss/base/_colors.scss';

$mq-breakpoints: (
    tablet: 768px,
    desktop: 1032px,
    wide: 1500px,
    maximum: 1730px
);

.mint {
  color: $mint;
}

a {
  color: #000000;
  text-decoration: none;
}

.input {
  width: 100%;
  height: 100%;
  max-height: 46px;
  padding: 7px 10px;
  border-radius: 4px;
  line-height: normal;
  line-height: inherit;
  border: 1px solid $grey; 
}

.content-area {
    width: 100%;
    padding: 0px 10px;
    @include mq($from: tablet) {
        padding: 0px 38px;
    }
    @include mq($from: desktop) {
        padding: 0px 50px;
    }
    @include mq($from: wide) {
        padding: 0px 72px;
    }
}

@font-face {
  font-family: 'MuseoSans';
  font-weight: normal;
  src: url('~static/fonts/MuseoSans/MuseoSansRegular.ttf'); /* IE9 Compat Mode */
  src: url('~static/fonts/MuseoSans/MuseoSansRegular.woff') format('woff'),
       url('~static/fonts/MuseoSans/MuseoSansRegular.eot') format('eot'),
}

.ft {
  float: left;
}

.row {
    width: 100%;
    &:after {
        content: "";
        display: table;
        clear: both;
        visibility: hidden;
        height: 0px;
        font-size: 0px;
    }
}

.page {
  display: flex;
  width: 100%;
  height: 100vh;
}
.page-body {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  flex-grow: 1;
  height: 100%;
}
html {
  font-family: "MuseoSans", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*, *:before, *:after {
  box-sizing: border-box;
  margin: 0;
}

.button--green {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #3b8070;
  color: #3b8070;
  text-decoration: none;
  padding: 10px 30px;
}

.button--green:hover {
  color: #fff;
  background-color: #3b8070;
}

.button--grey {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #35495e;
  color: #35495e;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 15px;
}

.button--grey:hover {
  color: #fff;
  background-color: #35495e;
}
</style>

