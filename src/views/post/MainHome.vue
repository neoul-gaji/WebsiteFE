<template lang="">
<div>
    <div class="nav">
        <NavBar/>
    </div>
    <div class="main">
        <div class="container">
            <div class="shout">
                <ul>
                    <li class="text">
                        <h1>당신의 메이트를 쉽고 빠르게 찾는 방법</h1>
                        <h3>위대한 시작을 여기에서</h3>
                    </li>
                    <li class="logo">
                        <img src="@/assets/logo.png" alt="logo">
                    </li>
                </ul>
            </div>
            <div class="card">
                <Card/>
                <Card/>
                <Card/>
                <Card/>
                <Card/>
                <Card/>
            </div> 
        </div>   
    </div>
</div>
</template>
<script>

import NavBar from '@/components/NavBar.vue'
import Card from '@/views/post/MainHomeCard.vue'
export default {
    data(){


    },
    methods: {

    },
    components: {
        'NavBar' : NavBar,
        'Card' : Card
    }
}

</script>

<style scoped>

    /* ----css reset---- */
    * {
      margin: 0;
      padding: 0;
    }

    .main {
        height: 100%;
        width: 100%;
        background-color: #EFF3F6; 
        padding-top: 55px;
    }

    .main > .container > .card {
        display: flex;
        flex-direction: row;
        flex-wrap: wrap;
        justify-content: center;
        border: none;
        background-color: #EFF3F6; 
        width: 1180px; /* navbar와 맞춤 */   
        position: relative;
        left: -30px;
        top: -80px;
    }
    
    .shout > ul > li {
        display: inline-block;
    }


    

    
</style>