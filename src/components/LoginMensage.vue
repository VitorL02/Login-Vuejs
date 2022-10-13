<template>
    <div class="left-login">
        <h1>Faça Login <br>E entre para nosso time</h1>
        <img :src="logo" alt="Logo">
    </div>
</template>

<script>
import logo from '../assets/climate-change-animate.svg'
export default {
    name: 'LoginMensage',
    setup() {
        return {
            logo
        }
    }
}

</script>


<style>
.left-login {
    width: 50vw;
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
}

.left-login>h1 {
    font-size: 3vw;
    color: #77ffc0
}

.left-login>img {
    width: 75%;
}

@media only screen and (max-width:600px) {

    .left-login>img {
        width: 100%;
    }

    .left-login>h1 {
        display: none;
    }

    .left-login {
        height: auto;
    }

}
</style>