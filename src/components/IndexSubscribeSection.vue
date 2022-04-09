<template>
    <div class="subscribe-section position-relative">
        <div class="container">

            <img src="../assets/img/maxcoach-shape-02.png" alt="Immagine sfondo" class="circle position-absolute">

            <img src="../assets/img/maxcoach-shape-02.png" alt="Immagine sfondo" class="second-circle position-absolute">

            <div class="row">
                <div class="col-12 text-center py-5">
                    <h1 class="d-inline-block mx-2">Subscribe</h1>
                    <h1 class="d-inline-block green-color">Newslettes</h1>
                </div>

                <div class="col-5 m-auto text-center mb-3">
                    <p>Enter your email address to register to our newsletter subscription delivered on a regular basis!</p>
                </div>
            </div>

            <div class="row">
                <div class="col-6 m-auto">
                    <div class="input-group mb-3">
                        <input type="text" class="form-control" placeholder="Enter your email">

                        <div class="input-group-append">
                            <button class="btn btn-outline-secondary p-3 green-background text-white" type="button"> <b>Subscribe</b> </button>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'IndexSubscribeSection',

}
</script>

<style lang="scss" scoped>
    .subscribe-section{
        height: 400px;
    }

    .circle {
        top: 50%;
        left: 15%;
        width: 100px;
    }

    .second-circle {
        top: 35%;
        right: 15%;
        width: 100px;
    }


</style>