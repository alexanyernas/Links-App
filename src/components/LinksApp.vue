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
            text: 'Sitio Web',
            icon: 'fas fa-globe',
            url: 'https://punicorp.com',
            styles: {
              color: '#FFF',
              background: '#441247'
            }
          },
          {
            text: 'Instagram',
            icon: 'fab fa-instagram',
            url: 'https://instagram.com/puni.corp',
            styles: {
              color: '#FFF',
              background: '#de1b85'
            }
          },
          {
            text: 'Telegram',
            icon: 'fab fa-telegram-plane',
            url: 'https://t.me/alegiannattasio',
            styles: {
              color: '#FFF',
              background: '#0088cc'
            }
          },
          {
            text: 'WhatsApp',
            icon: 'fab fa-whatsapp',
            url: 'https://wa.me/+584120137644',
            styles: {
              color: '#FFF',
              background: '#128C7E'
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
  background: linear-gradient(to bottom, rgba(0, 0, 0, 0.9), rgba(68, 18, 71, 0.5));
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