<template>
    <div class="woodsmokeBg pb-5">
        <div class="container pt-5">
            <div class="row pt-5">
                <div class="col-8 pt-5">
                    <div>
                        <h5 class="text-uppercase greenText fs-6">
                            send a message
                        </h5>
                        <h2 class="fs-1 fw-bolder text-white">
                            Get in
                            <span class="customBg">
                                Touch
                            </span>
                        </h2>
                        <p class="text-secondary">
                            we will respond at your message as soon as possible
                        </p>
                    </div>
                    <form action="#">
                        <div class="mb-3">
                            <div class="d-flex pb-3">
                                <input type="text" placeholder="Name" class="w-50 p-3">
                                <input type="email" placeholder="Email" class="ms-3 w-50 p-3">
                            </div>
                            <div class="d-flex">
                                <input type="number" placeholder="Phone" class="w-50 p-3">
                                <select class="text-secondary ms-3 form-select w-50" id="validationCustom04" required>
                                    <option selected disabled value="">More Info</option>
                                    <option>...</option>
                                </select>
                            </div>
                        </div>
                        <div class="mb-3">
                            <textarea class="w-100 p-3 pb-5" placeholder="Message" id="exampleFormControlTextarea1" rows="3"></textarea>
                        </div>
                        <div>
                            <button class="text-uppercase fw-bold btnGreen px-4" type="submit">
                                send
                            </button>
                        </div>
                    </form>
                </div>
                <div class="col-4">
                    <div>
                        <h4 class="text-white pb-3">
                            Example Inc.
                        </h4>
                        <p class="text-secondary">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Error fugit ullam.</p>
                        <p class="text-secondary">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Error fugit ullam.</p>
                        <div class="greenText fs-5">
                            <div class="pb-3">
                                 <i class="fa-solid fa-phone iconBg me-2 rounded-circle p-2"></i> <span>+1(305) 1234-5678</span>
                            </div>
                            <div class="pb-3">
                                <i class="fa-solid fa-envelope me-2 iconBg rounded-circle p-2"></i> <span>hello@example.com</span>
                            </div>
                            <div class="pb-3">
                                <i class="fa-solid fa-location-dot iconBg rounded-circle p-2 me-2"></i> <span>Main Avenue, 987</span>
                            </div>
                            <div>
                                <button class="text-uppercase btnLight ms-1 fs-6">
                                    view map
                                </button>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'FooterComp'
    }
</script>

<style scoped>
    .woodsmokeBg {
        background-color: #121117;
    }

    .customBg {
        background-color: #0E272D;
        padding: 0 10px;
        border-radius: 5px;
        font-weight: 900;
    }
    /* hide icons in input number */
    input::-webkit-outer-spin-button,
    input::-webkit-inner-spin-button {
    -webkit-appearance: none;
     margin: 0;
    }
    input,
    select,
    textarea{
        background-color: #1D1D23;
        border: none;
        color: white;
    }
    input:before{
        background-color: #1D1D23;
    }
    .iconBg{
        background-color: #0F2128;
    }
</style>