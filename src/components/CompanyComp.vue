<template>
    <div class="container-fluid">
        <div class="row">
            <div class="col-6">
                <div class="w-75 float-end">
                    <h5 class="text-uppercase about">
                    about the network
                </h5>
                <h2 class="py-4">
                    <span class="px-2 rounded-3 me-2">
                        The
                    </span>
                    Company
                </h2>
                <p class="text-secondary">
                    Lorem ipsum dolor sit amet, consectetur adipisicing elit. Provident beatae commodi accusantium, temporibus necessitatibus! Nisi, assumenda!
                </p>
                <div class="row row-cols-4">
                    <div>
                        <h2 class="ms-2 colorGreen fw-bolder">0</h2>
                        <h2>Employees</h2>
                        <p class="text-secondary">Lorem ipsum dolor sit amet.</p>
                    </div>
                    <div class="mx-3">
                        <h2 class="ms-2 colorGreen fw-bolder">0</h2>
                        <h2>Partners</h2>
                        <p class="text-secondary">Lorem ipsum dolor sit amet.</p>
                    </div>
                    <div>
                        <h2 class="ms-2 colorGreen fw-bolder">0</h2>
                        <h2>Customers</h2>
                        <p class="text-secondary">Lorem ipsum dolor sit amet.</p>
                    </div>
                </div>
                <div class="pt-5">
                    <button class="btnGreen">get in touch</button>
                    <button class="btnLight" style="color: #058283;">read more</button>
                </div>
                </div>
            </div>
            <div class="col-6 imgContainer">
                <img class="img-fluid h-100 w-100" src="./../assets/img/about-5.jpg" alt="">
            </div>
        </div>
    </div>
</template>

<script> 
</script>

<style scoped>
h5{
    font-weight: 800;
    color: #058283;
    font-size: 1em;
}
h2 span{
    background-color: #DAECED;
    color: #058283;
}
.colorGreen{
    color: #0ea5a5;
}
.imgContainer{
    height: 700px;
}
.col-6{
    padding: 0 !important;
}
.about{
    margin-top: 150px;
}
h2{
    font-weight: 900;
}
</style>