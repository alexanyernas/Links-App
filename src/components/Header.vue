<template>
    <header class="header">
        <div class="img"></div>
        <h3 class="title">Alexanyer Naranjo</h3>
        <p class="description">Desarrollador web con un gran amor por el aprendizaje ☕</p>
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
    margin-top: 15px;
    color: #FFF;

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
        font-family: cursive;
    }

    .description
    {
        font-family: cursive;
        margin-bottom: 15px;
    }
}
</style>