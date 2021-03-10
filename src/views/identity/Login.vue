// 로그인 창

<template lang="">
    <div id="container" class="d-flex flex-column justify-content-center">
        <div class="d-inline-flex align-items-center">
            <img src="@/assets/logo.png" alt="logo" id="logo-img">
            <h3>꿈꾸는 개발자</h3>
        </div>
       <p>새로운 도전, <strong>꿈꾸는 개발자</strong>와 함께</p>
       <form action="" id="form-container">
            <input type="text" name="id" placeholder="아이디" class="w-100 p-2">
            <input type="password" name="password" placeholder="비밀번호" class="w-100 p-2">
            <b-button type="submit" formmethod="POST" class="w-100 p-2">로그인</b-button>
        </form>
        <div class="d-flex justify-content-between align-items-center" id="form-additional-container">
            <b-form-checkbox value="valid-login" class="d-flex flex-column"></b-form-checkbox>
            <span style="margin-left:-45px">로그인 유지</span>
            <div>
                <router-link to="/apply-reset-id">아이디</router-link>
                <span> | </span>
                <router-link to="/apply-reset-password">비밀번호 찾기</router-link>
            </div>
        </div>
        <div id="register-link-form">
            <strong>새로운 도전을 꿈꾸시나요? </strong><router-link to="/register">회원가입</router-link>
        </div>
    </div>
</template>
<script>
export default {
    
}
</script>
<style scoped>

input:focus {
    outline: none;
}

a {
    text-decoration: none;
}

input {
    border :none;
    border-bottom: 2px solid #ec4c66;
    margin-bottom: 5px;
}

button:hover {
    background-color: #f07489;
}

button {
    background-color: #ec4c66;
    border : none;
}

#form-container {
    width: 300px;
}

#form-additional-container {
    font-size: 12px; 
    width: 250px; 
    margin:auto;
    margin-top: 15px;
    margin-bottom: 10px;
}

#logo-img {
    height: 100px;
}

#container {
    position: absolute;
    top:50%;
    left:50%;
    width: 300px;
    height: 350px;
    margin-left: -150px;
    margin-top: -175px;
    text-align:center
}
    
</style>