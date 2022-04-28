<template>
<main>
    <section class="bgLightGreen p-5">
        <div class="container pt-5">
            <div class="row">
                <CardComp
                v-for="elm,i in cards"
                :key="i"
                :elm="elm"
                />
            </div>
        </div>
    </section>
    <div class="d-flex justify-content-center clipContainer">
        <ClipComp/>
    </div>
</main>
</template>

<script>
import ClipComp from './ClipComp.vue'
import CardComp from './CardComp.vue'
export default{
    name: 'MainComp',
    data(){
        return{
            cards:[
                {
                    'fwClass': 'fa-user-group',
                    'title': 'Human Capital',
                    'description': 'Humanizing business: Harness the power of technology to improve the way peaple work.' 
                },
                {
                    'fwClass': 'fa-chart-pie',
                    'title': 'Core Business',
                    'description': 'It takes innnovative approaches to transform, modernize, and run existing platform.' 
                },
                {
                    'fwClass': 'fa-gauge-high',
                    'title': 'Performance',
                    'description': 'Achieving maximum impact and value from investiments in finance and supply chain.' 
                },
                
            ]
        }
    },
    components:{
        CardComp,
        ClipComp,
    }
}
</script>
<style scoped>
    .bgLightGreen{
        background-color: #e4eae6;
    }
    .clipContainer{
        margin-top: -30px;
    }
</style>