// 로그인 창

<template lang="">
    <div id="container" class="d-flex-column justify-content-center">
        <div class="d-inline-flex align-items-center">
            <img src="@/assets/logo.png" alt="logo" id="logo-img">
            <h3>꿈꾸는 개발자</h3>
        </div>
       <p>새로운 도전, <strong>꿈꾸는 개발자</strong>와 함께</p>
       <form action="">
            <input type="text" id="input-text" name="id" placeholder="아이디">
            <input type="text" id= "input-text" name="id" placeholder="비밀번호"> <br>
            <b-button>로그인</b-button>
        </form>
        <div class="d-flex justify-content-between" style="font-size: 12px;">
            <label><input type="checkbox"> 로그인 유지</label>
            <a href="">비밀번호/아이디 찾기</a>
        </div>
        <span>새로운 도전을 꿈꾸시나요? </span><a href="/register">회원가입</a>
    </div>
</template>
<script>
export default {
    
}
</script>
<style scoped>


#logo-img {
    height: 100px;
}

#container {
    position: absolute;
    top:50%;
    left:50%;
    width: 300px;
    height: 300px;
    margin-left: -150px;
    margin-top: -150px;
    text-align:center
}
    
</style>