<template>
    <div class="business-section section">
        <div class="container">
            <div class="row">
                <div class="col-7 left-side position-relative">
                    <div class="image-container position-absolute">
                        <img src="../assets/img/icon-youtube-play.png" alt="Logo Youtube" class="position-absolute">
                    </div>
                </div>

                <div class="col-5 right-side text-white">
                    <h2>To Thrive in Business Today, You'll Need a Good Plan
                    </h2>


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

    .container {
        height: 100%;
        background-image: url('../assets/img/home-business-hero-global-image.png');
        background-size: contain;
        background-repeat: no-repeat;
        background-position: right;
    }

    .image-container {
        width: 70%;
        height: 300px;
        background-image: url('../assets/img/home-business-video-poster-670x450.jpg');
        background-repeat: no-repeat;
        background-size: contain;
        top: 200px;
        left: 150px;

        & img {
            width: 80px;
            left: 50%;
            top: 50%;
            transform: translate(-50%, -50%);
        }
    }

    .right-side {
        background-image: url('');
        height: 500px;

    }
</style>