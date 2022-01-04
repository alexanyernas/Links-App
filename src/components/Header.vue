<template>
    <header class="header">
        <div class="img"></div>
        <h3 class="title">Punicorp</h3>
        <p class="description">Convertimos tus ideas en realidad. Contacta con nosotros ☕</p>
    </header>
</template>

<style lang="scss">
.header
{
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
    margin-top: 30px;
    color: #FFF;

    .img
    {
        width: 150px;
        height: 150px;
        background-repeat: no-repeat;
        background-image: url('../assets/Profile.png');
        background-position: center;
        background-size: 125px;
        border-radius: 50%;
        margin-bottom: 10px;
    }

    .title
    {
        margin-bottom: 10px;
    }

    .description
    {
        margin-bottom: 15px;
    }
}
</style>