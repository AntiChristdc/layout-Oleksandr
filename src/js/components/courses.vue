<template>
    <div>
        <div class="heading">
            <h2>Popular trainings</h2>
            <a href="#">See more</a>
        </div>
        <div class="courses">
            <div class="courses__item" v-for="el in courses" :key="el.title">
                <img :src="'img/' + el.img" :alt="el.title">
                <h2>{{ el.title }}</h2>
                <p>{{ el.cl }}</p>
                <div class="time">{{ el.time }}</div>
            </div>
        </div>
    </div>
</template>

<script>
 export default {
    props: ['data'],
    created() {
        this.courses = this.data
    },
    data( ) {
        return {
            courses: []
        }
    }
 }
</script>

<style lang="scss" scoped>
    .heading {
        display: flex;
        justify-content: space-between;
        align-items: center;
        margin-bottom: 35px;

        h1 {
            font-size: 2.1em;
        }

        a {
            text-transform: uppercase;
            font-size: 0.8em;
        }
    }

    .courses {
        margin-bottom: 150px;
        display: flex;
        flex-wrap: wrap;
        @media (min-width: 950px) {
            justify-content: space-between;
        }

        @media (max-width: 950px) {
            justify-content: center;
            flex-direction: column;
        }


        .courses__item {
            margin-top: 70px;
            cursor: pointer;
            position: relative;
            overflow: hidden;
            border-radius: 10px;

            @media (max-width: 950px) and (min-width: 430px) {
                margin-left: auto;
                margin-right: auto;
                width: 373px;
            }

            @media (max-width: 430px) {
                width: 100%;
            }

            .time {
                position: absolute;
                right: 0;
                bottom: 62px;
                background-color: black;
                padding: 5px;
                font-weight: 600;
                border-radius: 10px 0 0 0;
            }

            h2 {
                font-size: 2.5em;
                margin-left: 10px;
                position: relative;
                bottom: 35px;
                font-weight: 600;
            }

            p {
                color: #ababab;
                position: relative;
                bottom: 30px;
                margin-left: 10px;
                font-size: 0.9em;
            }

            img {
                opacity: 0.7;
                transition: all 400ms ease;
                &:hover {
                    opacity: 1;
                    scale: 1.1;
                }
                @media (max-width: 430px) {
                width: 100%;
                }
            }
        }
    }
</style>