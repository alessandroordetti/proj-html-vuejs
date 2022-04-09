<template>
    <main>
        <IndexJumbotron />

        <IndexApproachSection />

        <IndexFirstExploreSection />

        <IndexSecondExploreSection />

        <IndexBusinessSection />

        <IndexEventsSection />

        <IndexFeedbacksSection />

        <IndexSubscribeSection />
    </main>
</template>

<script>
import IndexJumbotron from './IndexJumbotron.vue';
import IndexApproachSection from './IndexApproachSection.vue';
import IndexFirstExploreSection from './IndexFirstExploreSection.vue';
import IndexSecondExploreSection from './IndexSecondExploreSection.vue';
import IndexBusinessSection from './IndexBusinessSection.vue';
import IndexEventsSection from './IndexEventsSection.vue';
import IndexFeedbacksSection from './IndexFeedbacksSection.vue';
import IndexSubscribeSection from './IndexSubscribeSection.vue';

export default {
    components: {
        IndexJumbotron,
        IndexApproachSection,
        IndexFirstExploreSection,
        IndexSecondExploreSection,
        IndexBusinessSection,
        IndexEventsSection,
        IndexFeedbacksSection,
        IndexSubscribeSection,
    }
}
</script>

<style>

</style>