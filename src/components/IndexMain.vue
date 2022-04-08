<template>
    <main>
        <IndexJumbotron />

        <IndexApproachSection />

        <IndexFirstExploreSection />

        <IndexSecondExploreSection />

        <IndexBusinessSection />
    </main>
</template>

<script>
import IndexJumbotron from './IndexJumbotron.vue';
import IndexApproachSection from './IndexApproachSection.vue';
import IndexFirstExploreSection from './IndexFirstExploreSection.vue';
import IndexSecondExploreSection from './IndexSecondExploreSection.vue';
import IndexBusinessSection from './IndexBusinessSection.vue';

export default {
    components: {
        IndexJumbotron,
        IndexApproachSection,
        IndexFirstExploreSection,
        IndexSecondExploreSection,
        IndexBusinessSection
    }
}
</script>

<style>

</style>