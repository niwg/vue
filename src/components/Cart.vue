<template>
    <div>
        <h2>我是购物车</h2>
        <table>
            <tr>
                <td>勾选</td>
                <td>课程名称</td>
                <td>课程单价</td>
                <td>数量</td>
                <td>课程总价</td>
            </tr>
            <tr v-for="(item) in courseItem" :key="item.id">
                <td></td>
                <td>{{item.name}}</td>
                <td>{{item.price}}</td>
                <td>{{item.number}}</td>
                <td>{{item.number * item.price}}</td>
            </tr>
        </table>
    </div>
</template>

<script>
    export default {
        props: ['courseItem']
    }
</script>

<style lang="scss" scoped>

</style>