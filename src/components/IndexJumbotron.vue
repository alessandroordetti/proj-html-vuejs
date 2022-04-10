<template>
    <div class="jumbotron section-background-gray section mb-5 position-relative">
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

        <div class="lateral-options position-absolute text-center fs-4 rounded-2">
            <i class="fas fa-caret-right d-block"></i>
            <i class="far fa-plus-square"></i>
            <i class="fas fa-book"></i>
            <i class="fas fa-shopping-cart"></i>

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

    .lateral-options {
        height: 135px;
        width: 35px;
        background-color: white;
        right: 0;
        top: 20%;
    }
</style>