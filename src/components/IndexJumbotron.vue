<template>
    <div class="jumbotron section-background-gray section mb-5">
        <div class="container d-flex position-relative">
            <div id="left-section">
                <h5>
                    New Challenges, New Skills
                </h5>

                <h1 class="text-uppercase fw-bold">
                    build your own life coaching business
                </h1>

                <p>Whole-Life Business Coaching for committed entrepreuners</p>

                <button class="rounded py-3 px-5 text-white fw-bold">
                    Get started today
                </button>
            </div>

            <div class="avatar-wrapper">
                <img src="../assets/img/home-business-hero-avatar.png" alt="Immagine avatar">
            </div>

        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped> 

    .container {
        height: 100%;
    }

    #left-section {
        width: 50%;
        height: 50%;
    }

    #left-section {
        margin: auto 12%;

        & h5 {
            color: #25ac94;
        }

        & button {
            background-color: #25ac94;
            border: transparent;
            font-size: .8rem;
        }

        & button:hover{
            background-color: #3f3a64;
        }
    }

    .avatar-wrapper {
        background-image: url('../assets/img/home-business-hero-global-image.png');
        background-size: cover;
        back
        
        .img {
        height: 600px;
        position: absolute;
        bottom: 0;
        right: 0;
        }
    }


</style>