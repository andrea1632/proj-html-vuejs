<template>
    <div class="container pb-5">
        <div class="text-center pt-5">
            <div class="text-uppercase pt-5">
                <strong class="colorGreen">we do more for everyone</strong>
            </div>
            <h2 class="text-white customFs pt-3">
                Actions & <span>Projects</span>
            </h2>
        </div>
        <nav class="pt-4">
            <ul class="row justify-content-around d-flex w-75 m-auto">
                <li class="col text-center py-5" v-for="elm,i in navMenu" :key="i">
                    <a class="text-uppercase" href="">{{navMenu[i]}}</a>
                </li>
            </ul>
        </nav>
        <div class="row justify-content-around pb-5">
            <div class="col-4 text-white customCard mb-5" v-for="elm,i in cards" :key="i" :style="{ backgroundImage: `url(${require('./../assets/img/' + elm.bgPath)})` }">
                <div class="w-100 h-100 overlay">
                    <h3>{{elm.description}}</h3>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default{
    name: 'ProjectComp',
    data(){
        return{
            'title': 'Action & Projects',
            'navMenu': ['all','institutional','social','events','innovation','environment','technology'],
            'cards': [
            {
                'bgPath': 'project-1.jpg',
                'description': 'Accademic professional program in social media'
            },
            {
                'bgPath': 'project-2.jpg',
                'description': "President's speech at the annual meeting"
            },
            {
                'bgPath': 'project-3.jpg',
                'description': 'International business trip in Shangai'
            },
            {
                'bgPath': 'project-4.jpg',
                'description': 'Technology workshop with education theme'
            },
            {
                'bgPath': 'project-5.jpg',
                'description': 'Donation of clothes and food to the partner NGO'
            },
            {
                'bgPath': 'project-6.jpg',
                'description': 'Confraternization of the procurement team'
            }
            ]
        }
    }
}
</script>

<style scoped>
    .customFs{
        font-size: 3em;
        font-weight: 900;
    }
    .colorGreen{
        color: #00A6A6;
    }
    ul{
        list-style: none;
    }
    a{
        text-decoration: none;
        color: white;
        padding: 15px 10px;
    }
    a:hover{
        color: white;
    }
    ul li:hover a{
        background-color: #0E272D;
        border-radius: 5px;
    }
    h2 span{
        background-color: #0E272D;
        padding: 0 7px;
        border-radius: 5px;
    }
    .customCard{
        width: 30%;
        border-radius: 20px;
    }
    .customCard h3{
        padding-top: 80%;
        text-align: center;
    }
    .col-4{
        padding: 0 !important;
    }
</style>