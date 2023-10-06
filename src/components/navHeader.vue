<template>
    <div>
        <header class="v-header-top">
            <div class="navbar-header px-4 pt-2 pb-2 d-flex">
                <img src="../assets/logo.png" class="basket__img"/>
                <h3 class="basket__text">Product Basket</h3> 
                <p class="app__version" >v{{ appVersion }}</p>
            </div>
        </header>
    </div>
</template>

<script>
    var pjson = require('../../package.json');
    export default {
        name:'navHeader',
        data() {
            return {
                appVersion : pjson.version,
            }
        }
    }
</script>

<style>
    .version {
        background-color: var(--default-color);
        margin-top: 1rem;
    }
    .v-header-top .navbar-header {
        padding: 0.2rem 0;
        margin-top: -3.1%;
    }
    .header-text{
    font-weight: 700 !important;
    }
    .navbar-header{
        background: #0E0A32;
        margin-top: -60px !important;
        width: 100vw;
        /* height: 70px; */
        display: flex;
        position: sticky;
        top: 0;
        z-index: 1000;
    }

    .app__version{
        color: white;
        font-size: 18px;
        margin-left: auto;
        margin-top: 12px;
        margin-right: 20px;
    }
    .basket__img {
        width: 40px; 
        height: 40px; 
        margin-top: 2px;
    }
    .basket__text {
        color:white; 
        padding: 5px; 
        margin-top: 6px;
    }
</style>