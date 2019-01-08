<template>
  <div>
    <site-content>
      <nav-bar
        :navData="navData"
        logoText="Medi Service Pvt. Ltd."
        logoSubtitle="Passion for quality care"
        class="horizon"
      />
    </site-content>
    <nuxt/>
  </div>
</template>

<script>
import NavBar from '~/components/Common/Header'
import SiteContent from '~/components/Elements/SiteContent'

export default {
  data() {
    return {
      navData: [
        {
          name: 'Our Service',
          link: '#'
        },
        {
          name: 'About',
          link: '#'
        },
        {
          name: 'Our Mission',
          link: '#'
        },
        {
          name: 'Team',
          link: '#'
        },
        {
          name: 'Clients',
          link: '#'
        },
        {
          name: 'Contact',
          link: '#'
        }
      ]
    }
  },
  components: {
    NavBar,
    SiteContent
  }
}
</script>

<style>
@font-face {
  font-family: Elephant;
  src: url(https://admin.esah.in/uploads/b7b79c3ba75545c6885fc942af334c31.TTF);
}

.elephant {
  font-family: 'Elephant';
  font-weight: 500;
}

* {
  padding: 0;
  margin: 0;
}

html {
  line-height: 1.4;
}

.site-container {
  width: 100%;
}

.horizon {
  padding-bottom: 16px;
  border-bottom: 2px solid black;
}

a,
a:link,
a:visited,
a:active,
a:hover {
  text-decoration: none;
}
a {
  font-family: 'Lato', sans-serif;
  text-transform: uppercase;
}
h1,
h2,
h3,
h4,
h5,
h6 {
  font-family: 'Lato', sans-serif;
}
p,
input,
textarea,
button {
  font-family: 'Lato', sans-serif;
}
</style>
