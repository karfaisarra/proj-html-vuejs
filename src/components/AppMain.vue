<script>
import JumbotronSection from './JumbotronSection.vue';
import BuildDream from './BuildDream.vue';
import ConstructAndCareer from './ConstructAndCareer.vue';
import StatisticalSection from './StatisticalSection.vue';
import LatestFeatured from './LatestFeatured.vue';
import LearnSection from './LearnSection.vue';
import EventsSection from './EventsSection.vue';
import LoveUs from './LoveUs.vue';

export default {
    name: 'AppMain',
    components: {
        JumbotronSection,
        BuildDream,
        ConstructAndCareer,
        StatisticalSection,
        LatestFeatured,
        LearnSection,
        EventsSection,
        LoveUs
    }
}

</script>
<template>
    <main>
        <JumbotronSection />
        <BuildDream />
        <ConstructAndCareer />
        <StatisticalSection />
        <LatestFeatured />
        <LearnSection />
        <EventsSection />
        <LoveUs />
    </main>
</template>
<style lang="scss" scoped>

</style>