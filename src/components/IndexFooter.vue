<template>
    <footer class="position-relative">
        <div class="container">
            <div class="row">
                <div class="col-5 text-white p-5">
                    <h5 class="fw-bold mb-3">Address</h5>

                    <p>382 NE 191st St # 87394 Miami, FL 33179-2899</p>

                    <p>+1(305)547-9909 (9am-5pm EST,Monday - Friday)</p>

                    <p>support@maxcoach.com</p>

                    <div class="img-container">
                        <i class="fab fa-facebook-square mx-3 fs-3"></i>
                        <i class="fab fa-twitter-square mx-3 fs-3"></i>
                        <i class="fab fa-instagram-square mx-3 fs-3"></i>
                        <i class="fab fa-linkedin mx-3 fs-3"></i>
                    </div>
                </div>

                <div class="col-7 text-white p-5 mb-5 d-flex">
                    <div class="explore mx-4">
                        <h5 class="fw-bold mb-3">Explore</h5>

                        <div class="uls-wrapper d-flex">
                            <div>                   
                                <ul v-for="(element, index) in exploreLeftOptions" :key=index>
                                    <li>{{element.option}}</li>
                                </ul>
                            </div>
                            
                            <div>
                                <ul v-for="(element, index) in exploreRightOptions" :key=index>
                                    <li >{{element.option}}</li>
                                </ul>
                            </div>
                        </div>
                    </div>

                    <div class="information">
                        <h5 class="fw-bold mb-3">Information</h5>
                        
                        <ul v-for="(element, index) in informationOptions" :key=index>
                            <li >{{element.option}}</li>
                        </ul>
                    </div>
                </div>

                <div class="col-4 m-auto text-center text-white">
                    <p><i class="far fa-copyright mx-2"></i>2020 Maxcoach. All Rights Reserved</p>
                </div>
            </div>
        </div>

        <div class="arrow-container green-background position-absolute text-white">
            <i class="fas fa-arrow-up fs-4"></i>
        </div>
    </footer>
</template>

<script>
export default {
    name: 'IndexFooter',
    data: function() {
        return {
            exploreLeftOptions: [
                {
                    option: 'Start here'
                },
                {
                    option: 'Blog'
                },
                {
                    option: 'About us'
                },
            ],
            exploreRightOptions: [
                {
                    option: 'Success story'
                },
                {
                    option: 'Courses'
                },
                {
                    option: 'Contact us'
                },
            ],
            informationOptions: [
                {
                    option: 'Membership'
                },
                {
                    option: 'Purchase guide'
                },
                {
                    option: 'Privacy policy'
                },
                {
                    option: 'Terms of service'
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
    footer {
        background-color: #323043;
        height: 400px;
    }

    .explore {
        width: 60%;
        height: 100px;
    }

    ul {
        list-style-type: none;
        padding: 0;
    }

    li {
        margin-right: 5rem;
    }

    .arrow-container {
        width: 60px;
        height: 60px;
        border-radius: 50%;
        line-height: 60px;
        text-align: center;
        right: 1rem;
        bottom: 1rem;
    }
</style>