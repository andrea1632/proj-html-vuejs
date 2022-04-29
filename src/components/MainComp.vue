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
    <section>
        <CompanyComp/>
    </section>
    <div class="d-flex justify-content-center clipContainer">
        <ClipComp/>
    </div>
    <section class="bgDarkBlue">
        <ProjectComp/>
    </section>
    <section class="pb-5 mb-5">
        <ProcessComp/>
    </section>
</main>
</template>

<script>
import ProcessComp from './ProcessComp.vue'
import ProjectComp from './ProjectComp.vue'
import ClipComp from './ClipComp.vue'
import CardComp from './CardComp.vue'
import CompanyComp from './CompanyComp.vue'
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
        CompanyComp,
        ProjectComp,
        ProcessComp
    }
}
</script>
<style scoped>
    .bgLightGreen{
        background-color: #e4eae6;
    }
    .clipContainer{
        position: absolute;
        left: 50%;
        transform: translate(-50%, -50%);
    }
    .bgDarkBlue{
        background-color: #111117;
    }
</style>