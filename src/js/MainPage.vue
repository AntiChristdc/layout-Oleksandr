<template>
    <Nav />
    <Head />
    <Courses :data="courses"/>
    <Features />
    <Videos />
    <Footer />
</template>

<script>
import Nav from './components/nav.vue'
import Head from './components/head.vue'
import Courses from './components/courses.vue'
import Features from './components/features.vue'
import Videos from './components/videos.vue'
import Footer from './components/footer.vue'

export default {
    components: {
        Nav, Head, Courses, Features, Videos, Footer
    },
    data() {
        return {
            courses: [
                {'title': 'Кардио', 'cl': '250 калорий', 'time': '58:24', 'img': 'cardio.png'},
                {'title': 'Растяжка', 'cl': '250 калорий', 'time': '58:24', 'img': 'stretch.png'},
                {'title': 'Йога', 'cl': '250 калорий', 'time': '58:24', 'img': 'joga.png'},
                {'title': 'Бег', 'cl': '250 калорий', 'time': '58:24', 'img': 'run.png'},
                {'title': 'Гантели', 'cl': '250 калорий', 'time': '58:24', 'img': 'metal.png'},
                {'title': 'На улице', 'cl': '250 калорий', 'time': '58:24', 'img': 'street.png'},
            ]
        }
    }
}
</script>

<style lang="scss">

</style>