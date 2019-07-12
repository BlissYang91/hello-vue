<template>
    <div>接口测试</div>
</template>

<script>

    export default{
        name:'catoon',
        data(){
            return{

            }
        },
        mounted(){
            this.getData();
        },
        methods:{
            async getData(){
                // let data  = a
                this.$axios.get('https://wanandroid.com/wxarticle/chapters/json')
                .then(response =>{
                    console.log('response : ', response.data)
                })
            }
        }
    }
    
</script>