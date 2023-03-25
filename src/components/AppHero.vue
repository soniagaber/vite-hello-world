<script></script>
<template>
    <div id="hero">
        <h2>Aggretsuko</h2>
    </div>
</template>
<style scoped>

#hero{
    margin: 20px auto;
    width: 800px;
    height: 500px;
    background-image: url("../../public/img/aggretsuko.webp");
    background-size: cover;
    position: relative;
    display: flex;
    justify-content: center;
    align-items: center;
}

#hero::before{
    content: "";
    position: absolute;
    top: 0;
    left: 0;
    background-color: rgba(0, 0, 0, 0.8);
    z-index: 2;
    height: 100%;
    width: 100%;
}

h2{
    color: orangered;
    position: absolute;
    text-transform: uppercase;
    z-index: 3;
    font-size: 2.5em;
    cursor: pointer;
    text-shadow: 5px 3px rgba(0, 0, 0, 0.8);
}

h2:hover{
    transform: scale(150%);
}

</style>