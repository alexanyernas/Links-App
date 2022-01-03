<template>
    <header class="header">
        <div class="img"></div>
        <h3 class="title">Punicorp</h3>
        <p class="description">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Iusto perspiciatis.</p>
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
        background-color: #FFF;
        background-image: url('../assets/Profile.png');
        background-position: center;
        background-size: 125px;
        border-radius: 50%;
        border: 3px solid #441247;
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