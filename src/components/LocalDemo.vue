<template>
    <div class="box">
        <div class="main">
            <button class="get_btn" @click="getList">不啊啊啊啊好</button>
        </div>
    </div>

</template>
<script>


export default{
    name:'LocalDemo',
    data() {
        return {
            title:'这里是TITLE',
            count: 1
        }
    },
    methods:{
        getList(){
            this.$Axios({
                method: 'get',
                url:'',
                params:{
                    limit: 1
                }
            }).then(res =>{
                console.log(res)
            })
        }
    }
}
</script>
