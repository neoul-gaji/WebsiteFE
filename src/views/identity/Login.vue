// 로그인 창

<template lang="">
    <div id="arpmain">
        <div>
          <div id="container">
            <img src="../../assets/nwgj.jpg" style="width: 100px; height: 100px; float: left " >
            <br>
            <br>
            <br>
            <h6 style="font-weight:bold; float: right">지금 개발에 도전해보세요!</h6>
            <div class="id">
              <input id="ID" type="text" name="ID" placeholder="아이디">
              <input id="Password" type="password" name="Password" placeholder="비밀번호">
              <input id="Login" type="submit" value="로그인">

                  <br>
                <div>
                    <label class="checkbox-inline" style="float: left; margin-left: 10px; ">
                        <input type="checkbox" id="inlineCheckbox1" value="option1">로그인 유지</label>

                    <p class="find"  style="float: right; ">
                        <a href="/" style="color:darkgrey;font-weight: bold;">아이디/비밀번호 찾기</a>
                    </p>

                </div>
                <br>
                <br>
                <div class ="register" style="text-align: center;">
                    <span style="color: lightslategrey;">000 은 처음이신가요? </span>
                    <a href="/Register" style="color:#42b983 ;font-weight: bolder;">회원가입</a>
                </div>

            </div>
            <router-view/>
          </div>
        </div>

      </div>
</template>
<script>
export default {



}

</script>
<style>



#arpmain {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}


#container {

  padding: 50px;
  position: relative;
  top: 120px;
  margin: 24px auto;
  width: 480px;

}


#ID{
  padding:8px;
  line-height: 24px;
  border: 1px solid #ededed;
  color: #292929;
  font-size: 16px;
  background-color: #f9f9f9;
  display: block;
  box-sizing: border-box;
  width: 100%;
  height: 40px;
  border-radius: 12px;
  font: 400 14px Arial;
}

#Password{
  padding:8px;
  line-height: 24px;
  border: 1px solid #ededed;
  color: #292929;
  font-size: 16px;
  background-color: #f9f9f9;
  display: block;
  box-sizing: border-box;
  width: 100%;
  height: 40px;
  border-radius: 12px;
  font: 400 14px Arial;
  margin-top: 8px;

}
#Login {
  border: 0;
  color: #fff;
  font-size: 16px;
  font-weight: bold;
  background-color:  #42b983;
  margin-top: 8px;
  display: block;
  box-sizing: border-box;
  width: 100%;
  height: 40px;
  border-radius: 12px;
  letter-spacing: -0.5px;
}

#checkbox-inline {

    float:left;
}

</style>
