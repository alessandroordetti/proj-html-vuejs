<template>
    <main>
        <IndexJumbotron />

        <IndexApproachSection />

        <IndexExploreSection />
    </main>
</template>

<script>
import IndexJumbotron from './IndexJumbotron.vue';
import IndexApproachSection from './IndexApproachSection.vue';
import IndexExploreSection from './IndexExploreSection.vue'

export default {
    components: {
        IndexJumbotron,
        IndexApproachSection,
        IndexExploreSection
    }
}
</script>

<style>

</style>