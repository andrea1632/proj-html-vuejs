<template>
    <div class="py-5">
         <div class="text-center pt-5">
            <h4 class="text-uppercase greenText fs-6 fw-bolder">
                customer testimonials
            </h4>
            <h2 class="py-3 fw-bolder">
                Trusted
                <span class="ps-3 greenBg greenText p-1 fs-1 rounded pe-3">
                    Feedback
                </span>
            </h2>
            <p class="text-secondary pb-5 pt-2">
                We work innovative methodologies to ensure that the entire reformatting process is done <br>
                from start to finish as planned.
            </p>
        </div>
        <div class="container pb-5">
            <div class="row gx-4">
                <div class="px-5 py-4 col bg-white mx-3 customCard d-flex flex-column" v-for="elm, i in cards" :key="i">
                    <div class="imgContainer">
                        <img class="img-fluid pb-4" :src="`${elm.pathToLogo}`" alt="">
                    </div>
                    <div>
                        <p class="text-secondary">{{elm.description}}</p>
                        <p class="text-secondary pb-2">{{elm.lorem}}</p>
                    </div>
                    <i class="fa-solid fa-quote-right align-self-end"></i>
                </div>
            </div>
        </div>
    </div>
</template>

<script> 
export default{
    name: 'CustomerComp',
    data(){
        return{
            cards: [
                {
                    'pathToLogo': require('./../assets/img/logo-1.png'),
                    'description': 'Praesent volutpat justo sit amet elementum malesuda. Praesent sagittis augue justo, in accumsan orci rhoncus at pellentesque.',
                    'lorem': 'lorem ipsum dolor sit amet, consecteur adipiscing elit.'
                },
                {
                    'pathToLogo': require('./../assets/img/logo-2.png'),
                    'description': 'Praesent volutpat justo sit amet elementum malesuda. Praesent sagittis augue justo, in accumsan orci rhoncus at pellentesque.',
                    'lorem': 'lorem ipsum dolor sit amet, consecteur adipiscing elit.'
                },
                {
                    'pathToLogo': require('./../assets/img/logo-3.png'),
                    'description': 'Praesent volutpat justo sit amet elementum malesuda. Praesent sagittis augue justo, in accumsan orci rhoncus at pellentesque.',
                    'lorem': 'lorem ipsum dolor sit amet, consecteur adipiscing elit.'
                },
            ]
        }
    }
}
</script>
    
<style scoped>
.customCard{
    border-radius: 10px;
}
i{
    color: #CCCCCC;
    font-size: 2em;
}
</style>