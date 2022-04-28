<template>
    <div class="col bg-white p-5 mx-2 rounded-3">
        <div class="iconContainer rounded-circle">
            <i class="fa-solid" :class="elm.fwClass"></i>
        </div>
        <h3 class="pt-3">
            {{elm.title}}
        </h3>
        <p class="py-5">
            {{elm.description}}
        </p>
    </div>
</template>
<script>
export default {
    name: 'CardComp',
    props: ['elm']
}
</script>
<style scoped>
.iconContainer{
    background-color: #DAECED;
    display: inline-block;
    padding: 20px;
}
i{
    font-size: 1.3em;
    color: #058283;
}
h3{
    font-weight: 600;
}
</style>