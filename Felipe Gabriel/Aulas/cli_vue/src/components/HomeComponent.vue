<template>
    <div>
        <header>
            <p>Seja bem vindo: {{nome}} </p>
            <img width=largura height=altura :src="urlImgMeishoDoto" alt="Imagem">
        </header>
    </div>
</template>

<script>
export default {
    name: "HomeComponent",
    data() {
        return {
            nome: "Felipe",
            urlImgMeishoDoto: "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcS1aWgcx9ugxKHh44VsyD90ZCl8v5yZp5YsnOwoT-s_JQ&s=10",
            altura: 200,
            largura: 200,
        };
           },
        mounted() {
            setTimeout(() => {
                this.urlImgMeishoDoto = "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTyETndrL7NVMmzCiC7Tu9dHTinhYcwlFUlN6oxzpXkVEnpkAk97C9hlkQ&s=10";
            }, 5*1000);
        }
    };
</script>
