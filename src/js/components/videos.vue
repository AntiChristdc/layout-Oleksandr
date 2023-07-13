<template>
<div class="videos">
    <div class="video" @click="videos[0] = !videos[0]">
        <p class="number">01</p>
        <div class="info">
            <h4>Упражнения дома</h4>
            <p>15 видео</p>
        </div>
        <div class="icon"><i class="fa-solid fa-arrow-right"></i></div>

        <div class="video__open" v-if="videos[0]">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Laborum enim laudantium exercitationem, tempore quod consectetur aliquam, voluptatibus impedit repudiandae autem velit nostrum facere harum dicta aspernatur perspiciatis. Doloremque, perferendis sint.
        </div>

    </div>
    <div class="video" @click="videos[1] = !videos[1]">
        <p class="number">02</p>
        <div class="info">
            <h4>Оставайтесь в форме</h4>
            <p>48 видео</p>
        </div>
        <div class="icon"><i class="fa-solid fa-arrow-right"></i></div>

        <div class="video__open" v-if="videos[1]">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. 
            Laborum enim laudantium exercitationem, tempore quod 
            consectetur aliquam, voluptatibus impedit repudiandae 
            autem velit nostrum facere harum dicta aspernatur perspiciatis. 
            Doloremque, perferendis sint.
        </div>

    </div>
    <div class="video" @click="videos[2] = !videos[2]">
        <p class="number">03</p>
        <div class="info">
            <h4>Интенсив</h4>
            <p>25 видео</p>
        </div>
        <div class="icon"><i class="fa-solid fa-arrow-right"></i></div>

        <div class="video__open" v-if="videos[2]">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. 
            Laborum enim laudantium exercitationem, tempore quod 
            consectetur aliquam, voluptatibus impedit repudiandae 
            autem velit nostrum facere harum dicta aspernatur perspiciatis. 
            Doloremque, perferendis sint.
        </div>

    </div>
    <div class="video" @click="videos[3] = !videos[3]">
        <p class="number">04</p>
        <div class="info">
            <h4>Простые упражнения</h4>
            <p>35 видео</p>
        </div>
        <div class="icon"><i class="fa-solid fa-arrow-right"></i></div>

        <div class="video__open" v-if="videos[3]">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. 
            Laborum enim laudantium exercitationem, tempore quod 
            consectetur aliquam, voluptatibus impedit repudiandae 
            autem velit nostrum facere harum dicta aspernatur perspiciatis. 
            Doloremque, perferendis sint.
        </div>

    </div>
    <div class="video" @click="videos[4] = !videos[4]">
        <p class="number">05</p>
        <div class="info">
            <h4>Сжигание калорий</h4>
            <p>35 видео</p>
        </div>
        <div class="icon"><i class="fa-solid fa-arrow-right"></i></div>

        <div class="video__open" v-if="videos[4]">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. 
            Laborum enim laudantium exercitationem, tempore quod 
            consectetur aliquam, voluptatibus impedit repudiandae 
            autem velit nostrum facere harum dicta aspernatur perspiciatis. 
            Doloremque, perferendis sint.
        </div>

    </div>
</div>
</template>

<script>
export default {
    data() {
            return {
                videos: [false, false, false, false, false]
            }
    }
}
</script>

<style lang="scss" scoped>

.videos {
    @media(min-width: 1100px) {
        margin-top: 300px;
    }
    @media(max-width: 1100px) {
        margin-top: 200px;
    }
}
.video {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 40px 0;
    cursor: pointer;
    transition: all 300ms ease;
    flex-wrap: wrap;
    i {
        transition: all 300ms ease;
        margin-right: 10px;
    }

    &:not(:last-of-type) {
        border-bottom: 0.5px solid #666666;
    }

    &:hover {
        background-color: #212121;

        i {
            transform: rotate(90deg);
        }
    }

    .info {
        width: 450px;

        @media(min-width: 630px) {
            width: 450px;
        }
        @media(max-width: 630px) {
            width: 200px;
        }
    }

    .number {
        color: #575757;
        font-weight: 600;
        font-size: 1.2em;
    }

    h4 {
        font-size: 2.5em;
        font-weight: 400;

        @media(min-width: 630px) {
            font-size: 2.5em;
        }
        @media(max-width: 630px) {
            font-size: 1.5em;
        }
    }

    p {
        color: #575757;
        margin-top: 10px;
    }

    .video__open {
        text-align: center;
        margin-top: 15px;
        padding: 5px 10px;
        background-color: #222222;
        border-radius: 10px;
    }

}
</style>