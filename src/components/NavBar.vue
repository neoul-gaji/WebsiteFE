<template lang="ko">
  <div class="fixed-top d-flex justify-content-center align-items-center shadow-sm rounded" style="background:#f8fbfe; height:100px;">
    <nav class="d-flex justify-content-between align-items-center m-2">
      <div id="nav-container-left" class="d-inline-flex justify-content-between align-items-center">
        <router-link to="/home" class="d-inline-flex align-items-center">
          <img src="@/assets/logo.png" alt="logo" id="logo-name">
          <ul>
            <li style="font-size: 11px;">성균관대의</li>
            <li style="font-size: 23px;">꿈꾸는개발자들</li>
          </ul>
        </router-link>
        <span>|</span>
        <span><router-link to="#" id="location">모집글작성</router-link></span>
      </div>
      <ul id="nav-cotainer-right" class="d-inline-flex justify-content-between align-items-center">
          <li>팀원 찾기</li>
          <li>멘토 찾기</li>
          <li>모집글작성</li>
          <li><b-icon icon="bell-fill" scale="1.5"></b-icon></li>
          <li><b-icon icon="person-circle" scale="1.5"></b-icon></li>
          <li><b-icon icon="unlock-fill" scale="1.5"></b-icon></li>
      </ul>
    </nav>
  </div>
</template>
<script>
// $(".nav").width($(window).width());

export default {
    
}
</script>
<style scoped>
/* css reset */
nav {
  padding: 10px;
  width: 1180px;
}

ul {
  list-style:none;
  padding-left: 0px;
  margin-bottom: 0px;
}

a {
  color: black;
}


#logo-name {
  width: 50px;
  height: 50px;
}

#nav-container-left {
  width: 330px;
}

#nav-cotainer-right {
  width: 450px;
}




</style>