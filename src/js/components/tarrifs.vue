<template>
    <div>
        <h3>Тарифы</h3>
        <div class="tarrifs">
            <div>
                <h4>Free</h4>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam.</p>
                <ul>
                    <li>Lorem ipsum dolor sit amet</li>
                    <li>Quis nostrud exercitation ullamco</li>
                    <li>Exercitation ullamco</li>
                    <li>Lorem ipsum dolor sit amet</li>
                    <li>Excepteur sint occaecat excepteur sint occaecat</li>
                    <li>Sed ut perspiciatis unde omnis</li>
                </ul>
                <span><a href="#">More</a>  <i class="fa-solid fa-arrow-right"></i></span>
            </div>
            <div>
                <h4>Plus+</h4>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam.</p>
                <ul>
                    <li>Lorem ipsum dolor sit amet</li>
                    <li>Quis nostrud exercitation ullamco</li>
                    <li>Exercitation ullamco</li>
                    <li>Lorem ipsum dolor sit amet</li>
                    <li>Excepteur sint occaecat excepteur sint occaecat</li>
                    <li>Sed ut perspiciatis unde omnis</li>
                    <li>Exercitation ullamco</li>
                    <li>Lorem ipsum dolor sit amet</li>
                </ul>
                <button>Join us</button>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
h3 {
    margin: 70px 0;
    font-size: 3em;
    font-weight: 400;
}

.tarrifs {
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
    margin-bottom: 150px;

    >div {
        @media (min-width: 750px){width: 35%}
        background-color: #232532;
        color: #A8A7A8;
        padding: 50px 5%;

        &:last-of-type {
            background-color: #323443;
            color: #ADACAE;
            @media (max-width: 750px){margin-top: 30px}
        }

        h4 {
            color: white;
            text-align: center;
            font-size: 2em;
            margin-bottom: 30px;
        }

        ul {
            margin: 20px 30px;
        }

        span {

            a {
                color: #0070C9;
                &:hover {
                color: #41a9ff;
                }
            }

            i {
                margin-left: 9px;
                font-size: 1.2em;
            }
        }

        button {
            background-color: #0070C9;
            border: none;
            border-radius: 10px;
            color: white;
            padding: 5px 10px;
            cursor: pointer;
            transition: all 400ms ease;

            &:hover {
                background-color: #41a9ff;
                transform: scale(1.1);
                color: black;
            }
        }
    }
}
    
</style>