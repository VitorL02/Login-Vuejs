<template>
    <div class="card">
        <Inputs></Inputs>
    </div>
</template>


<script>

import Inputs from './Inputs.vue';

export default {
    name: 'CardLogin',
    components: {
        Inputs
    }
}

</script>

<style>
.card {
    width: 60%;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    padding: 30px 35px;
    background: #2f2841;
    border-radius: 20px;
    box-shadow: 0px 10px 40px #00000056;
}

@media only screen and (max-width:600px) {


    .card {
        width: 100%;
        height: auto;
    }

}
</style>