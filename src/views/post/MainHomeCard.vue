<template lang="ko">
    <div class="card">
        <ul class="card-inner" href="#">
            <li><a class="card-image"><img src="https://picsum.photos/600/300/?image=25" alt="image"></a></li>
            <li><a class="card-title">{{title}}</a></li>
            <li><a class="card-inform">
                <ul>
                    <li><a class="team-name set-gray">{{teamname}}</a></li>
                    <li><a class="eye" style="color: black;"><b-icon icon="eye" scale="1.5"></b-icon></a></li>
                    <li><a class="eye-num set-gray">{{viewer}}</a></li>
                    <li><a class="talk" style="color: black;"><b-icon icon="card-text" scale="1.5"></b-icon></a></li>
                    <li><a class="talk-num set-gray">{{talk}}</a></li>
                </ul>
                </a></li><br>
            <li><a class="purpose">{{purpose}}</a></li>
            <li><a class="inner-top set-gray">{{teamnow}}</a></li>
            <li><a class="inner-top set-gray">{{locationdue}}</a></li><br>
            <li><a class="foot">
                <ul>
                    <a class="time">{{time}} 시간전</a>
                    <a class="tag" style="color: black;"><b-icon icon="tag" scale="1.5"></b-icon></a> 
                    <!-- li로 씌우면 개별 float 안먹음 주의 -->
                </ul>
                </a></li>
        </ul>
    </div>
</template>
<script>
export default {
    data(){
        return {
            title: '스타트업 공모전 팀원 모집',
            teamname: '너울가지',
            viewer: 80,
            talk: 4,
            purpose: '창업팀 멤버',
            teamnow: '엔지니어링/아이디어 구상단계/구성원 2명',
            locationdue: '서울특별시 성동구/~모집시까지',
            time: 20
        }
    }
    
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
    .card-inner > li > a {
        text-decoration: none;
    }
    .card-inner > li > ul > li > a {
        text-decoration: none;
    }
    /* ----END css reset---- */
    .card {
        border: 1px solid rgba(0, 0, 0, 0.1);
        border-radius: 30px;
        box-shadow: 3px 3px rgba(0, 0, 0, 0.1);
        z-index: 1000;
        width: 90%;
        margin: 20px;
    }
    
    @media(min-width:992px){
        .card {
            width: 350px;
        }
    }
    
    .card:hover {
        box-shadow: 3px 3px 3px 3px rgba(0, 0, 0, 0.1);
    }


    .card.show{
        display: inline-block;
    }
    .card-image > img {
        width: 100%;
        height: 100px;
        margin-bottom: 15px;
        transform: scale(1);
        -webkit-transform: scale(1);
        -moz-transform: scale(1);
        -ms-transform: scale(1);
        -o-transform: scale(1);
        transition: all 0.8s ease-in-out;
    }

    .card-image > img:hover {
        transform: scale(1.1);
        -webkit-transform: scale(1.1);
        -moz-transform: scale(1.1);
        -ms-transform: scale(1.1);
        -o-transform: scale(1.1);
    }

    img {
      width: 30px;
      height: 30px;
    }
    .card-inner {
        float: center;
        margin: 30px;
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
        font-size: 18px;
        color: black;
    }
    .purpose {
        font-size: 18px;
        color: black;
    }
    .time {
        color: black;
        font-size: 15px;
    }
    .set-gray {
        color: rgba(0, 0, 0, 0.6);
        font-size: 15px;
    }
    
</style>