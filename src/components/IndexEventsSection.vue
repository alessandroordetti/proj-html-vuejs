<template>
    <div class="events-section section">
        <div class="container">
            <div class="row text-center">
                <div class="col py-5">
                    <h5 class="green-color">Wanna transform your life?</h5>

                    <h1>Upcoming Events</h1>
                </div>
            </div>

            <div class="row">
                <div class="col-6 mb-5 " v-for="(element, index) in events" :key=index>
                    <div class="card-event d-flex justify-content-between bg-light" >
                        <div class="left-side m-4">
                            <h5> <i class="fas fa-map-marker-alt"></i> {{element.city}}</h5>

                            <h3>{{element.event}}</h3>
                        </div>

                        <div class="right-side text-center p-4">
                            <h2 class="green-color">{{element.day}}</h2>

                            <h4>{{element.month}}</h4>

                            <button class="px-3 py-1 rounded green-background text-white">Get ticket</button>
                        </div>
                    </div>
                </div>
            </div>

            <div class="row">
                <div class="col-6 m-auto text-center">
                    <span>Excited about our event?</span>

                    <span class="green-color">
                        View all events ->
                    </span>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'IndexEventsSection',

    data: function() {
        return {
            events: [
                {
                    city: 'Texas, US',
                    event: 'Storytelling Workshop',
                    day: '22',
                    month: 'Nov'
                },
                {
                    city: 'New York, US',
                    event: 'Painting Art Contest 2020',
                    day: '10',
                    month: 'Oct'
                },
                {
                    city: 'Hamburg, Germany',
                    event: 'International Art Fair 2020',
                    day: '23',
                    month: 'Nov'
                },
                {
                    city: 'Illinois, US',
                    event: 'Street Performance: Call for Artist',
                    day: '15',
                    month: 'Dec'
                },
                {
                    city: 'Illinois, US',
                    event: 'Consumer Food Safety Education Conference',
                    day: '22',
                    month: 'Jul'
                },
                {
                    city: 'Dubai',
                    event: 'How meditation improve your mental health?',
                    day: '12',
                    month: 'Aug'
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
    button {
        border: transparent;
    }

    .left-side {
        width: 320px;
    }
</style>