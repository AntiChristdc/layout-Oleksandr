<template>
    <div>
        <Nav />
        <HeadTarrifs />
        <HowTo />
        <Info />
        <Tarrifs />
        <Footer />
    </div>
</template>

<script>
import Nav from './components/nav.vue'
import HeadTarrifs from './components/HeadTarrifs.vue'
import HowTo from './components/howto.vue'
import Info from './components/info.vue'
import Tarrifs from './components/tarrifs.vue'
import Footer from './components/footer.vue'

export default {
    components: { Nav, HeadTarrifs, HowTo, Info, Tarrifs, Footer },
}
</script>

<style lang="scss" scoped>

</style>