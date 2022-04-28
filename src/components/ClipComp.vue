<template>
    <div class="clipBox">
        <div class="greenPoint rounded-circle" v-for="elm,i in 36" :key="i">

        </div>
    </div>
</template>
<script>
export default{
    name: 'ClipComp'
}
</script>
<style>
    .greenPoint{
        height: 10px;
        width: 10px;
        background-color: #B3E1DB;
        margin-right: 5px;
        margin-bottom: 5px;
    }
    .clipBox{
        display: flex;
        flex-wrap: wrap;
        width: 135px;
    }
</style>