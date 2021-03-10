/<template lang="">
    <div>
        <div id="create-post-container">
            <NavBar/>
            <div id="container" class="container shadow-lg">
                <div id="post-container" class="d-flex flex-column">
                    
                    <span>제목</span>
                    <input type="text">
                    <span>팀 한줄 설명</span>
                    <input type="text">
                    <div>
                        <span>팀 유형 </span>
                        <input type="text">
                    </div>
                    <div>
                        <span>모집 마감일 </span>
                        <input type="date">
                    </div>
                    <div>
                        <span>개발 분야 </span>
                        <input type="text">
                    </div>
                    <span>팀 이름</span>
                    <input type="text">
                    <div>
                        <span>공개 범위 </span>
                        <b-form-checkbox value="me">학교</b-form-checkbox>
                        <b-form-checkbox value="me">지역</b-form-checkbox>
                    </div>
                    
                    <span>팀 상세 설명</span>
                    <textarea name="" id="" cols="30" rows="10"></textarea>
                    <span>바라는 점</span>
                    <textarea name="" id="" cols="30" rows="10"></textarea>
                    <div>
                        <b-button>d</b-button>
                        <b-button>d</b-button>
                    </div>
                </div>
            </div>
        </div>
        <footer class="container">
            <div class="d-flex justify-content-center">
                hi
            </div>
         </footer>
    </div>
</template>
<script>
import NavBar from '@/components/NavBar.vue'

export default {
    components: {
        NavBar
    }
}

</script>
<style scoped>

#post-container {
    padding: 50px;
}

#create-post-container {
    margin-top:100px; 
    padding:70px 0px 100px 0px;
    background:#eff3f6;
}

#container {
    width: 880px;
    height: 1050px;
    background: white;
    margin-bottom: 100px;
}
</style>