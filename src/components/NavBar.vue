<template lang="ko">
<nav>
  <nav id="top_gnb">
    <ul class="top-nav-left">
      <li><a class="nwgj" href="#">NWGJ</a></li>
      <li><a class="illusion"></a></li>
      <li><a class="mate" href="#">메이트모집</a></li>
    </ul>
    <ul class="top-nav-right">
      <li><a class="nav-top-mini" href="#"><img src="@/assets/glass.jpg" alt="glass"></a></li>
      <li><a class="nav-top-mini" href="#"><img src="@/assets/message.jpg" alt="message"></a></li>
      <li><a class="nav-top-mini" href="#"><img src="@/assets/bell.jpg" alt="jingle"></a></li>
      <li><a class="nav-top-mini" href="#"><img src="@/assets/user.jpg" alt="user"></a></li>
    </ul>
  </nav>
  <nav id="bottom_gnb">
    <ul class="bottom-nav">
      <li><a class="bottom-filter" href="#"><img src="@/assets/filter.png" alt="filter"></a></li>
      <li><a class="illusion"></a></li>
      <li><a class="bottom-location" href="#">지역 &#9660;</a></li>
      <li><a class="illusion"></a></li>
      <li><a class="bottom-major" href="#">분야 &#9660;</a></li>
      <li><a class="illusion"></a></li>
      <li><a class="bottom-date" href="#">날짜 &#9660;</a></li>
      <li><a class="illusion"></a></li>
    </ul>
  </nav>
</nav>
</template>
<script>
export default {
    
}
</script>
<style scoped>
    /* ----css reset---- */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    li {
      list-style: none;
    }
    a {
      text-decoration: none;
    }
    /* ----END css reset---- */

    nav {
      width: auto;
      height: 60px;
      z-index: 2000;
      left: 0;
      right: 0;
      position: absolute;
    }
    #bottom_gnb {
      top: 60px; /* nav의 height와 동일한 값을 준다 */
    }
    .top-nav-left {
      float: left;
    }
    .top-nav-right {
      float: right;
    }
    .top-nav-left > li > .nwgj {
      display: inline-block;
      height: 36px;
      color: #EC4C66;
      font-size: 30px;
      font-weight: 600;
    } 
    .top-nav-left > li > .mate {
      font-weight: 600;
      color: rgba(0, 0, 0, 0.5);
    }
    .top-nav-left > li {
      display: inline-block;
    }
    .top-nav-right > li {
      display: inline-block;
    }
    .top-nav-left > li > a {
      line-height: 60px;
      padding: 0 30px;
      color: rgba(0, 0, 0, 0.9);
    }
    .top-nav-right > li > a {
      line-height: 60px;
      padding: 0 30px;
    }
    #top_gnb {
      border-bottom: 2px solid rgba(0, 0, 0, 0.3);
    }
    #bottom_gnb {
      border-bottom: 2px solid rgba(0, 0, 0, 0.3);
      float: left;
    }
    .bottom-nav > li {
      display: inline-block;
    }
    .bottom-nav > li > a {
      line-height: 60px;
      padding: 0 30px;
      color: rgba(0, 0, 0, 0.9);
      position: relative;
      top: -10px;
    }
    .bottom-nav > li > a > img {
      position: relative;
      top: -5px;
    }
    .bottom-nav > li > .bottom-filter {
      padding: 0;
    }
    /* illusion: 박스가 다 어긋나서 선을 만드는데 어려움이 있었음. illusion으로 선만들었음 */
    .top-nav-left > li > .illusion {
      width: 1px;
      padding: 0 1px;
      border-right: 2px solid rgba(0, 0, 0, 0.3);
      position: relative;
      top: -3px;
    }
    .bottom-nav > li > .illusion {
      width: 1px;
      height: 25px;
      padding: 16px 1px;
      border-right: 2px solid rgba(0, 0, 0, 0.3);
      position: relative;
    }
    /* ENN illusion */

    img {
      width: 80px;
      height: 80px;
    }
    .top-nav-right > li > a > img {
      width: 40px;
      height: 40px;
    }
    /* 미디어쿼리 적용 후 :hover 만들기 */
</style>