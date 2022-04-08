<template>
    <div class="explore-section section-background-gray ">
        <div class="container">
            <div class="row">
                <div class="col-12 text-center py-5">
                    <h2>
                        Let's Dream Big Together
                    </h2>

                    <h1 class="mb-5">
                        Explore How can I help you
                    </h1>
                </div>
            </div>

            <div class="row text-center">
                <div class="col-4" v-for="(element, index) in coachingOptions" :key=index>
                    <div class="card mb-5">
                        <img class="card-img-top" :src="element.image" alt="Logo persone durante coaching">
                        <div class="card-body">
                            <h3>{{element.title}}</h3>
                            <p>{{element.description}}</p>
                        </div>
                        <div class="discover">
                            <span class="fw-bold">Discover now -> </span>
                        </div>
                    </div>
                </div>
            </div>

            <div class="row">
                <div class="col-4 m-auto text-center">
                    <span class="dot bg-dark"></span>
                    <span class="dot mx-3"></span>
                    <span class="dot"></span>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'IndexExploreSection',

    data: function() {
        return {
            coachingOptions: [
                {
                    title: 'Consultative Training',
                    description: 'With a coach addressing multiple issues that are off abalance, affecting your business in various unconsidered ways',
                    image: require('@/assets/img/home-business-service-slide-01-480x298.jpg')
                },
                {
                    title: 'Real Deal Coaching',
                    description: 'Brings an exceptionally powerful opportunity. Being able to accept, to work with that opportunity.',
                    image: require('@/assets/img/home-business-service-slide-02-480x298.jpg')
                },
                {
                    title: 'Advisor Training Program',
                    description: 'Getting high quality, entrepreuner mindset driven online business coaching, is what is needed.',
                    image: require('@/assets/img/home-business-service-slide-03-480x298.jpg')
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
    h2 {
        color: #25ac94;
    }

    .card {
        height: 500px;

        & .discover {
            border-top: 1px solid lightgray;
            height: 50px;

            & span {
                line-height: 50px;
                color: #25ac94;
            }
        }
    }

    .dot {
    height: 15px;
    width: 15px;
    background-color: #bbb;
    border-radius: 50%;
    display: inline-block;
    }
</style>