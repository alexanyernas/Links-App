<template>
  <div class="body">
    <div class="container">
      <main class="main">
        <Header />
        <div 
          class="links" 
          v-for="(link, index) in links" 
          :key="index"
        >
          <Link 
            :text="link.text" 
            :icon="link.icon" 
            :url="link.url"
            :styles="link.styles"
          />
        </div>
        <Footer />
      </main>
    </div>
  </div>
</template>

<script>
import Header from './Header.vue'
import Link from './Link.vue'
import Footer from './Footer.vue'

export default {
    name: 'LinksApp',
    components: {
      Header,
      Link,
      Footer
    },
    data () {
      return {
        links: [
          {
            text: 'GitHub',
            icon: 'fab fa-github',
            url: 'https://github.com/alexanyernas/',
            styles: {
              color: '#FFF',
              background: '#333'
            }
          },
          {
            text: 'Instagram',
            icon: 'fab fa-instagram',
            url: 'https://instagram.com/alexanyernas',
            styles: {
              color: '#FFF',
              background: '#de1b85'
            }
          },
          {
            text: 'TikTok',
            icon: 'fab fa-tiktok',
            url: 'https://www.tiktok.com/@alexanyernaranjo/',
            styles: {
              color: '#FFF',
              background: '#EE1D52'
            }
          },
          {
            text: 'Twitter',
            icon: 'fab fa-twitter',
            url: 'https://twitter.com/alexanyernas/',
            styles: {
              color: '#FFF',
              background: '#00acee'
            }
          },
          {
            text: 'YouTube',
            icon: 'fab fa-youtube',
            url: 'https://www.youtube.com/c/AlexanyerNaranjo',
            styles: {
              color: '#FFF',
              background: '#c4302b'
            }
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
  font-family: 'Poppins', sans-serif;
}

*,
*::before,
*::after
{
  box-sizing: border-box;
}

body
{
  background-image: url('../assets/Background.jpg');
  background-position: center;
  background-size: cover;
}

.container
{
  padding: 32px;
  background: linear-gradient(to bottom, rgba(0, 0, 0, 0.3), rgba(0, 0, 0, 0.8));
  min-height: 100vh;  
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
  width: 50%;
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