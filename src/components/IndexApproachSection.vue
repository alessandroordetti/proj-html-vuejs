<template>
    <div class="approach section">
        <div class="container ">
            <div class="row">
                <div class="col-9 mb-5 text-center m-auto">
                    <h5>
                        Let's dream big together
                    </h5>

                    <h2 class="fw-bold">
                        We are pioneers of the digital approach, using leading-edge technology to simplify procedures and apply executive coaching in the new age of digitalization.
                    </h2>
                </div>

                <div class="col-4 cards-section d-flex p-3 mb-3" v-for="(element, index) in coachingOptions" :key=index >
                    <div class="info-card" >
                        <h2> {{element.title}} </h2>

                        <p> {{element.text}} </p>
                    </div>
                </div>

                <div class="col-12 d-flex justify-content-center">
                    <button class="left-button rounded py-3 px-5 fw-bold mx-3">Learn more</button>
                    <button class="right-button rounded py-3 px-5 text-white fw-bold mx-3">Get started today</button>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'IndexApproachSection',

    data: function () {
        return {
            coachingOptions: [
                {
                    title: 'One to One',
                    text: 'Getting the necessary clarity about the current state to help you improve your game.'
                },
                {
                    title: 'Anywhere',
                    text: 'Access to valuable and portable program which allow you to setup and live anywhere you want.'
                },
                {
                    title: 'On Time',
                    text: 'Punctually is our top priority because it\'s an essential criteria to assess a program quality.'
                },
                {
                    title: 'Online Courses',
                    text: 'Online business coaching now offers you a very powerful way to empower your business into success.'
                },
                {
                    title: 'Consulting',
                    text: 'You will get a clear sense of direction for your business, through assessment and faster results.'
                },
                {
                    title: 'Self Development',
                    text: 'Business Coaching often your focus and develop you both in a professional and personal way.'
                },
            ]
        }
    }
}
</script>

<style style="scss" scoped>
    h5, .left-button {
        color: #25ac94;
    }

    h1 {
        width: 80%;
        margin: 0 auto;
        line-height: 3.5rem;
    }

    .right-button {
        background-color: #25ac94;
    }

    .right-button:hover{
        background-color: #3f3a64;
    }

    .left-button:hover{
        background-color: #3f3a64;
        color: white;
    }

    button {
        border: transparent;
    }
</style>