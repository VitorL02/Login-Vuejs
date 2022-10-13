<template>
    <div class="login">
        <CardLogin></CardLogin>
    </div>
</template>


<script>
import CardLogin from './CardLogin.vue';

export default {

    name: 'LoginInputs',
    components: {
        CardLogin
    }
}
</script>

<style>
.login {
    width: 50vw;
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
}
</style>