<template>
    <header class="header">
        <div class="img"></div>
        <h4 class="title">Alexanyer Naranjo</h4>
        <p class="description">Desarrollador Web con una gran pasión por el aprendizaje, el café y las galletas ☕</p>
    </header>
</template>

<script>
export default {
    name: 'Header'
}
</script>

<style lang="scss">
.header
{
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
    margin-top: 45px;

    .img
    {
        width: 150px;
        height: 150px;
        background-image: url('../assets/Photo.jpg');
        background-position: center;
        background-size: cover;
        border-radius: 50%;
        margin-bottom: 10px;
    }

    .title
    {
        margin-bottom: 10px;
    }

    .description
    {
        font-size: 16px;
        margin-bottom: 15px;
    }
}
</style>