<template>
        <div class="explore-section section">
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

                <div class="row">
                    <div class="col-3 single-card position-relative mb-3" v-for="(element, index) in cards" :key=index>
                        <img :src="element.image" alt="Poster-card image">

                        <div class="description position-absolute">
                            <h5>{{element.price}}</h5>
                            <h4 class="text-white fs-5">{{element.title}}</h4>
                        </div>
                    </div>

                    <div class="col-5 m-auto text-center ">
                        <p>Take the control of their life back and start doing things to make their dream come true <span class="underlined "><strong>View all courses -></strong></span></p>
                    </div>
                </div>
            </div>
        </div>
</template>

<script>
export default {
    name: 'IndexSecondExploreSection',
    data: function () {
        return {
            cards: [
                {
                    price: '$40.00',
                    title: 'Learning to write as a Professional Author',
                    image: require('../assets/img/course-02-443x600.jpg')
                },
                {
                    price: 'Free',
                    title: 'Customer-centeric Info-Tech Strategies',
                    image: require('../assets/img/stock-full-hd-03-443x600.jpg')
                },
                {
                    price: '$19.00',
                    title: 'Open Programming Courses for Everyone: Python',
                    image: require('../assets/img/stock-full-hd-04-443x600.jpg')
                },
                {
                    price: '$26.00',
                    title: 'Academic Listening and Note-taking',
                    image: require('../assets/img/stock-full-hd-06-443x600.jpg')
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

    .single-card img {
        height: 400px;
        margin-right: 2rem;
        width: calc(100% - 4px) / 4;
    }

    .description {
        bottom: .2rem;
        padding: 1rem;
        width:90%;

        & h5 {
            color: #25ac94;
        }

    .underlined {
        text-decoration: underline;
    }
    }
</style>