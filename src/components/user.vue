<template>
    <div>
        <h1>User</h1>
        <p>我是user组件</p>
        <p>我是User的动态部分{{userId}}</p>
    </div>
</template>
<script>
export default {
    data(){
        return{
            userId:``
        }
    },
    watch:{
        $route(to,from){// to表示的是你要去的那个组件，from 表示的是你从哪个组件过来的，它们是两个对象，你可以把它打印出来，它们也有一个param 属性
        alert(111)
            console.log(to);
            console.log(from);
            this.userId = to.params.id
        }
    }
}
</script>
<style scoped>

</style>


