/<template lang="">
    <div id="create-post-container">
        <NavBar/>
        <div id="container" class="container shadow-lg">
            <div id="post-container">
                <h1>Hi</h1>
            </div>
        </div>
        <footer>
            hi
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
    padding-top:70px;
}

#container {
    width: 880px;
    height: 1300px;
    background: white;
    margin-bottom: 100px;
}
</style>