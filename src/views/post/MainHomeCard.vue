<template lang="">
    <div class="card">
        <ul class="card-inner" href="#">
            <li><a class="card-image"><img src="https://picsum.photos/600/300/?image=25" alt="image"></a></li>
            <li><a class="card-title">스타트업 공모전 팀원 모집</a></li>
            <li><a class="card-inform">
                <ul>
                    <li><a class="team-name set-gray">너울가지</a></li>
                    <li><a class="eye"><img src="@/assets/eye.png" alt="eye"></a></li>
                    <li><a class="eye-num set-gray">80</a></li>
                    <li><a class="talk"><img src="@/assets/message.jpg" alt="talk"></a></li>
                    <li><a class="talk-num set-gray">2</a></li>
                </ul>
                </a></li><br>
            <li><a class="purpose">창업팀 멤버</a></li>
            <li><a class="inner-top set-gray">엔지니어링/아이디어 구상단계/구성원 2명</a></li>
            <li><a class="inner-top set-gray">서울특별시 성동구/~모집시까지</a></li><br>
            <li><a class="foot">
                <ul>
                    <a class="time">2시간전</a>
                    <a class="tag"><img src="@/assets/tag.jpg" alt="tag"></a> 
                    <!-- li로 씌우면 개별 float 안먹음 주의 -->
                </ul>
                </a></li>
        </ul>
    </div>
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
    .card {
        border: 1px solid rgba(0, 0, 0, 0.1);
        border-radius: 30px;
        box-shadow: 3px 3px rgba(0, 0, 0, 0.1);
        z-index: 1000;
        width: 700px;
    }
    .card-image > img {
        width: 100%;
        height: 200px;
        margin-bottom: 15px;
    }
    img {
      width: 30px;
      height: 30px;
    }
    .card-inner {
        float: center;
        margin: 40px;
    }
    .card-inner > li > .card-inform > ul > li {
        display: inline-block;
        color: black;
    }
    .card-inner > li > .foot > ul > a {
        display: inline-block;
    }
    .card-inner > li > .foot > ul > .tag {
        float: right;
    }
    
    .card-inner > li > .card-inform > ul > li > .team-name {
        margin-right: 50px;
        position: relative;
        top: 2px; /* 눈깔이랑 위치 맞추면서 추후 조정 */
    }
    .card-inner > li > .card-inform > ul > li {
        margin-right: 10px;
    }
    .card-title {
        font-size: 1.2em;
        color: black;
    }
    .purpose {
        font-size: 1.2em;
        color: black;
    }
    .time {
        color: black;
    }
    .set-gray {
        color: rgba(0, 0, 0, 0.5);
    }
    

</style>