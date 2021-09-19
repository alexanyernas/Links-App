<template>
  <div class="container">
    <main class="main">
      <Header />
      <div class="links" v-for="(link, index) in links" :key="index">
        <Link 
          :text="link.text" 
          :icon="link.icon" 
          :url="link.url"
        />
      </div>
    </main>
  </div>
</template>

<script>
import Header from './Header.vue'
import Link from './Link.vue'

export default {
    name: 'LinksApp',
    components: {
      Header,
      Link
    },
    data () {
      return {
        links: [
          {
            text: 'Facebook',
            icon: 'fab fa-facebook',
            url: 'https://facebook.com/alexanyernas/'
          },
          {
            text: 'GitHub',
            icon: 'fab fa-github',
            url: 'https://github.com/alexanyernas/'
          },
          {
            text: 'Instagram',
            icon: 'fab fa-instagram',
            url: 'https://instagram.com/alexanyernas'
          },
          {
            text: 'Twitter',
            icon: 'fab fa-twitter',
            url: 'https://twitter.com/alexanyernas/'
          }
        ]
      }
    }
}
</script>

<style>
*
{
  margin: 0;
  padding: 0;
  font-family: 'Lato', sans-serif;
}

*,
*::before,
*::after
{
  box-sizing: border-box;
}

.container
{
  padding: 32px;
}

.main
{
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 45%;
}

@media only screen and (max-width: 600px)
{
  .main
  {
    width: 80%;
  }
}

.links
{
  width: 100%
}
</style>