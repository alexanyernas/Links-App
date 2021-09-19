<template>
  <div class="container_link">
    <a class="link" :href="url"><i :class="icon"></i><span>{{text}}</span></a>
  </div>
</template>

<script>
export default {
    name: 'Link',
    props: {
      text: String,
      icon: String,
      url: String
    }
}
</script>

<style lang="scss">
.link
{
  display: inline-block;
  padding: 15px;
  border: 2px solid #000;
  margin-bottom: 12px;
  border-radius: 15px;
  text-decoration: none;
  color: #000;
  width: 100%;
  text-align: center;

  i
  {
    position: absolute;
    left: 25px;
    font-size: 20px;
  }
}
</style>
