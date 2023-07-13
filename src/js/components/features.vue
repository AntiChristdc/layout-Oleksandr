<template>
    <div>
        <div class="features">
            <div class="features__heading">
                <img src="/img/yellow-line.svg" alt="yellow-line">
                <h3>Trainings special for you</h3>
            </div>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua consectetur adipiscing.</p>
            <button>Begin</button>
        </div>
        <div class="pictures">
            <div>
                <img src="/img/trener-1.png" alt="">
                <h4>Саманта Вильям</h4>
                <p>Trainer</p>
            </div>
            <div class="middle">
                <img src="/img/trener-2.png" alt="">
                <h4>Алина Реймонд</h4>
                <p>Trainer</p>
            </div>
            <div class="big">
                <img src="/img/trener-3.png" alt="">
                <h4>Джонатан Вайз</h4>
                <p>Trainer</p>
            </div>
        </div>
    </div>
</template>

<script>

</script>

<style lang="scss" scoped>
.features {
    width: 1500px;
    background-color: #191919;
    position: relative;
    padding: 120px 5% 270px 15%;

    @media (min-width: 1380px) {
        margin-left: 391px;
    }

    @media (max-width: 1380px) and (min-width: 1100px) {
        margin-left: 191px;
    }

    @media (min-width: 1100px) {
        padding: 120px 5% 270px 15%;
    }

    @media (max-width: 1100px) {
        padding: 50px
    }

    p {
        color: #ababab;
        line-height: 170%;

        @media (min-width: 1100px) {
            margin-left: 200px;
        }

        @media (min-width: 560px) {
            font-size: 1.3em;
            width: 500px;
        }

            @media (max-width: 560px) {
            font-size: 1.05em;
            width: 250px;
        }

    }

    button {
        background: #25AB75;
        padding: 20px;
        width: 160px;
        font-weight: 600;
        font-size: 1.02em;
        color: #fff;
        border: 0;
        cursor: pointer;
        border-radius: 10px;
        margin-top: 50px;
        transition: transform 500ms ease;

        @media (min-width: 1100px) {
            margin-left: 200px;
        }

        &:hover {
            transform: translateY(-7px);
        }
    }
    .features__heading {

        @media (min-width: 1100px) {
            position: absolute;
            left: -250px;
            top: 0;
        }


        h3 {
            font-size: 4.5em;
            width: 500px;

            @media (min-width: 1100px) {
                position: relative;
                top: -100px;
            }

            @media (min-width: 560px) {
                font-size: 4.5em;
                width: 500px;
            }

            @media (max-width: 560px) {
                font-size: 2.3em;
                width: 300px;
            }
        }

        img {

            @media (min-width: 1100px) {
                position: relative;
                top: 330px;
            }

        }
    }
}


.pictures {
    margin-bottom: 100px;
    display: flex;

    @media (min-width: 1380px) {
        padding-left: 70px;
    }

    @media (max-width: 1380px) and (min-width: 1100px) {
        position: relative;
        left: -127px;
    }

    @media (max-width: 1100px) {
        flex-wrap: wrap;
        justify-content: space-between;
    }

    > div {
        overflow: none;


        @media (min-width: 1100px) {
            position: relative;
        }

        @media (max-width: 1100px) {
            margin-top: 100px;
        }

        &.middle {
            top: 321px
        }

        &.big {
            top: -193px;

            h4, p {
                margin-left: 20px;
            }
        }

        h4 {
            font-weight: 400;
        }

        p {
            color: #ababab;
            font-size: 0.9em;
        }

        img {

            @media (max-width: 600px) {
            width: 90%;
        }
            opacity: 0.8;
            transition: all 400ms ease;
            &:hover {
                    opacity: 1;
                    scale: 1.05;
                    border-radius: 25px;
                }
        }
    }

}
</style>