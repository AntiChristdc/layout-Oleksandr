<template>
    <div>
        <h2>Не знаете с чего начать?</h2>
        <p>Программы предлагают ежедневные рекомендации в интерактивном календаре</p>
        <div class="blocks" :style="'left: ' + left + 'px'">
            <div class="item">
                <h3>Видео тренировки</h3>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit</p>
                <i class="fas fa-arrow-right"></i>
            </div>
            <div class="item">
                <h3>Программа курса</h3>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit</p>
                <i class="fas fa-arrow-right"></i>
            </div>
            <div class="item">
                <h3>Тарифы</h3>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit</p>
                <i class="fas fa-arrow-right"></i>
            </div>
            <div class="item">
                <h3>Полный доступ</h3>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit</p>
                <i class="fas fa-arrow-right"></i>
            </div>
            <div class="item">
                <h3>Видео тренировки</h3>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit</p>
                <i class="fas fa-arrow-right"></i>
            </div>
            <div class="item">
                <h3>Программа курса</h3>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit</p>
                <i class="fas fa-arrow-right"></i>
            </div>
            <div class="item">
                <h3>Тарифы</h3>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit</p>
                <i class="fas fa-arrow-right"></i>
            </div>
        </div>
        <div class="arrows">
            <img src="/img/arrow-next.svg" v-if="this.left != 0" @click="moveBlock('prev')" alt="">
            <img src="/img/arrow-next.svg" v-if="this.left >= -1900" @click="moveBlock('next')" class="next" alt="">
        </div>
    </div>
</template>

<script>
 export default {
    data() {
        return {
            left: 0,
        }
    },
    methods: {
        moveBlock(value) {
            let add = 330;
            if(value == 'next' && this.left != -1980) {
                this.left -= add
            } else if (value == 'prev' && this.left != 0) {
                this.left += add
            }
        }
    }
 }
</script>

<style lang="scss" scoped>
    h2 {
        margin-top: 80px;
        font-size: 2.4em;
    }

    p {
        color: #9b9a97;
        margin-top: 15px;
    }

    .blocks {
        display: flex;
        margin-top: 35px;
        margin-bottom: 60px;
        width: 2500px;
        position: relative;
        transition: all 400ms ease-in-out;

        .item {
            background-color:#323443;
            padding: 30px 25px;
            border-radius: 12px;
            width: 250px;

            &:not(:last-of-type) {
                margin-right: 30px;
            }

            p {
                color: #9b9a97;
            }

            i {
                float: right;
                font-size: 1.2em;
                position: relative;
                bottom: 30px;
            }
        }
    }

    .arrows {
        margin-bottom: 150px;
        img {
            transition: all 400ms ease;
            cursor: pointer;
            margin-right: 30px;

            &:hover {
                transform: scale(1.1);
            }

            &.next {
                transform: rotate(180deg);
                &:hover {
                transform: scale(1.1) rotate(180deg);
                }
            }
        }
    }
</style>