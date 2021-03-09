// 로그인 창

<template lang="">
    <div id="container" class="d-flex-column justify-content-center">
        <div class="d-inline-flex align-items-center">
            <img src="@/assets/logo.png" alt="logo" id="logo-img">
            <h3>꿈꾸는 개발자</h3>
        </div>
       <p>새로운 도전, <strong>꿈꾸는 개발자</strong>와 함께</p>
       <form action="" id="form-container">
            <input type="text" name="id" placeholder="아이디" class="w-100 p-2">
            <input type="text" name="password" placeholder="비밀번호" class="w-100 p-2">
            <button type="submit" formmethod="POST" class="w-100 p-2">로그인</button>
        </form>
        <div class="d-flex justify-content-between" id="form-additional-container">
            <label><input type="checkbox"> 로그인 유지</label>
            <div>
                <a href="">비밀번호</a>
                <span> | </span>
                <a href="">아이디 찾기</a>
            </div>
        </div>
        <strong>새로운 도전을 꿈꾸시나요? </strong><a href="/register">회원가입</a>
    </div>
</template>
<script>
export default {
    
}
</script>
<style scoped>

input[type="text"]:focus {
    outline: none;
}

a {
    text-decoration: none;
}

input[type="text"] {
    border :none;
    border-bottom: 2px solid #ec4c66;
    margin-bottom: 5px;
}

button {
    background-color: #4b4b68;
    border: none;
    border-radius: 7px;
    color : white;
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