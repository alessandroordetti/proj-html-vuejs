<template>
    <div class="business-section section position-relative">
        <img src="../assets/img/maxcoach-shape-07-100x100.png" alt="Immagine sfondo pallini" class="pallini position-absolute">

        <div class="container">
            <div class="row">
                <div class="col-7 left-side position-relative">
                    <div class="image-container position-relative position-absolute">
                        <img src="../assets/img/icon-youtube-play.png" alt="Logo YouTube" class="logo position-absolute">
                    </div>
                </div>

                <div class="col-5 right-side text-white m-auto">
                    <h2 class="mb-5">To Thrive in Business Today, You'll Need a Good Plan
                    </h2>

                    <h5 class="mb-4 text-open">
                        <i class="far fa-arrow-alt-circle-up"></i> How can we help?
                    </h5>

                    <p class="mb-5">Lorem ipsum dolor sit amet consectetur adipisicing elit. Harum, eius? Eveniet totam assumenda numquam, autem eum ea, ad eius maxime iste ipsa aperiam ipsam animi et aliquid ex necessitatibus quis?</p>

                    <h5 class="mb-5">
                        <i class="far fa-arrow-alt-circle-down"></i> Why would I need a business COACH?
                    </h5>

                    <h5 class="mb-5">
                        <i class="far fa-arrow-alt-circle-down"></i> What is one-on-one coaching?
                    </h5>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'IndexBusinessSection'
}
</script>

<style lang="scss" scoped>
    .business-section {
        background-color: #323043;
    }

    .container, .row, .left-side, .image-container {
        height: 100%;
    }

    .pallini {
        bottom: 100px;
        left: 200px;
    }

    .left-side > .image-container {
        height: 500px;
        width: 600px;
        top: 50%;
        transform: translate(0, -50%);
        background-image: url('../assets/img/home-business-video-poster-670x450.jpg');
        background-size: contain;
        background-repeat: no-repeat;

        & .logo {
            top:50%;
            left: 50%;
            transform: translate(-50%, -100%);
        }
    }

    .right-side {
        background-image: url('../assets/img/home-business-hero-global-image.png');
        background-size: contain;
        background-repeat: no-repeat;
        background-position: center;
    }

    .text-open {
        color: #25ac94;
    }


</style>