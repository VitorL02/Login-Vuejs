<template>
    <form @submit.prevent="save">
        <h1>LOGIN</h1>
        <div class="text-field">
            <label for="Usuario">Usuario</label>
            <input type="text" placeholder="Usuario" name="usuario" v-model="login.email">
        </div>

        <div class="text-field">
            <label for="Senha">Senha</label>
            <input type="password" placeholder="Senha" name="senha" v-model="login.password">
        </div>
        <button class="btn-login">Login</button>
    </form>
</template>



<script>

export default {
    name: 'LoginInputs',

    data() {
        return {
            login: {
                email: '',
                password: '',
            }
        }
    },
    methods: {
        save() {
            console.log(this.login);
            this.login = ''
        }
    }

}

</script>

<style>
h1 {
    color: #00ff88;
    text-align: center;
    font-weight: 800;
    margin: 0;
}

.text-field {
    width: 100%;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: center;
    margin: 10px 0;
}

.text-field>input {
    border: none;
    width: 100%;
    padding: 15px;
    border-radius: 10px;
    background: #514869;
    color: #f0ffde;
    font-size: 12pt;
    box-shadow: 0px 10px 40px #00000056;
    outline: none;
    box-sizing: border-box;
}

.text-field>label {
    color: #f0ffde;
    margin-bottom: 10px;
}

.text-field>input::placeholder {
    color: #f0ffffde;
}

.btn-login {
    width: 100%;
    padding: 16px 0px;
    margin-top: 10px;
    border: none;
    border-radius: 8px;
    outline: none;
    text-transform: uppercase;
    font-weight: 800;
    letter-spacing: 3px;
    color: #2b134b;
    background: #00ff88;
    cursor: pointer;
    box-shadow: 0px 10px 40px -12px #00ff8052;
}

.btn-login:hover {
    background: #00e77b;
}
</style>