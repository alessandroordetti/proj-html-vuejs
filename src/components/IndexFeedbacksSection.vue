<template>
    <div class="feedback-section section section-background-gray">
        <div class="container-fluid">
            <div class="row">
                <div class="col-8 m-auto text-center py-5">
                    <h5 class="green-color">
                        People are praising Maxcoach
                    </h5>

                    <h1>
                        What make they love us?
                    </h1>
                </div>
            </div>

            <div class="row p-5">
                <div class="col-4 px-5 py-3 card-wrapper rounded" v-for="(element, index) in users" :key=index>
                    <div class="feedback-card">
                        <h5>{{element.shortFeedback}}</h5>
                        <p class="mb-4">Lorem ipsum dolor sit amet consectetur adipisicing elit. Nam repudiandae accusamus doloribus quos, animi quo, quidem ut hic eos, excepturi consequatur delectus officia nihil tempore impedit temporibus aliquam molestias. Optio?</p>

                        <div class="user d-flex">
                            <img :src="element.image" :alt="element.name" >

                            <div class="user-name">
                                <h5>
                                    {{element.name}}
                                </h5>

                                <span>
                                    {{element.position}}
                                </span>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <div class="row">
                <div class="col-4 m-auto text-center mb-4">
                    <span class="dot mx-1 bg-dark"></span>
                    <span class="dot mx-1"></span>
                    <span class="dot mx-1"></span>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'IndexFeedbacksSection',
    data: function () {
        return {
            users: [
                {
                    shortFeedback: 'It\'s a coiche of quality for people with special needs',
                    image: require('../assets/img/testimonial-avata-03.jpg'),
                    name: 'Florence Themes',
                    position: '/ Multimedia Admin'
                },
                {
                    shortFeedback: 'High Level of efficiency and scientific teaching methods',
                    image: require('../assets/img/testimonial-avata-02.jpg'),
                    name: 'Mina Hollace',
                    position: '/ Freelancer'
                },
                {
                    shortFeedback: 'Professional team of specialists and passionate mentors at reach',
                    image: require('../assets/img/testimonial-avata-01.jpg'),
                    name: 'Madley Pondor',
                    position: '/ It Specialist'
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
    img {
        width: 75px;
        height: 75px;
        border-radius: 50%;
        margin-right: 2rem;
    }

    .card-wrapper:hover {
        background-color: white;
    }

    .dot {
    height: 15px;
    width: 15px;
    background-color: #bbb;
    border-radius: 50%;
    display: inline-block;
    }
</style>