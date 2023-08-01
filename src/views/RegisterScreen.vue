<template>
    <div>
        <h2>Registro de usuários:</h2>
        <hr>

        <div class="columns is-centered">
            <div class=" column is-half">
                <p>Nome: </p>
                <input type="text" placeholder="Nome do usuário" class="input" v-model='name'>
                <p>Email: </p>
                <input type="email" placeholder="E-mail" class="input" v-model='email'>
                <p>Senha: </p>
                <input type="password" placeholder="******************" class="input" v-model='password'>
                <br><br>
                <button class="button is-success" @click="register">Registrar</button>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data(){
        return{
            name : '',
            password : '',
            email : '',
        }
    },
    methods:{
        register(){
            console.log(this.name);
        }
    }
}
</script>

<style scoped>

</style>
