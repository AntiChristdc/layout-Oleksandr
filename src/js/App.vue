<template>
    <div class="wrapper">
        <div class="container">
            <router-view></router-view>
        </div>
    </div>
</template>

<script>

</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@200;300;400;600;800&display=swap');

$maincolor: #000000;
$textcolor: #fff;
$additionalcolor: #25AB75;

::selection {
    background: $additionalcolor;
}

* {
    margin: 0;
    padding: 0;
}

body {
    background-color: $maincolor;
    color: $textcolor;
    font-family: 'Poppins', sans-serif;
    font-weight: 400;
    font-size: 1em;
}

a {
    color: #ababab;
    text-decoration: none;
    transition: color 200ms ease;

    &:hover {
        color: $textcolor;
    }
}

.wrapper {
    overflow: hidden;
}

.container {

    @media(min-width: 1500px) {
        width: 1300px;
        margin: 0 auto;
    }
    @media(max-width: 1500px) and (min-width: 900px) {
        width: 80%;
        margin: 0 10%;
    }
    @media(max-width: 900px) {
        width: 90%;
        margin: 0 5%;
    }
}

</style>