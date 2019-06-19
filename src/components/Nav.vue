<template>
    <div> 
        <!-- <h2>Nav Bar</h2>  -->
        <nav> 
            <router-link class="spacing" 
                        v-for="link in links"
                        :key="link.id"
                        :to="`${ link.page }`">{{ link.text }} </router-link>

            <!-- <router-link to="/home">Home</router-link>
            <router-link to="/about">About</router-link>
            <router-link to="/contact">Contact</router-link> -->
        </nav> 
    </div>
</template>

<script>
export default {
  name: 'Nav', 
  data(){
    return {
      links: [ 
          // objects that specify the ID, what text to display, and the path to go to
          {
              id: 0,
              text: 'Hello World',
              page: '/HelloWorld'
          },
          {
              id: 1,
              text: 'Home',
              page: '/home'
          },
          {
              id: 2,
              text: 'About',
              page: '/about'
          },
          {
              id: 3,
              text: 'Contact',
              page: '/contact'
          }
      ]
    }
  }
}
</script>

<style>
nav:hover {
    background-color: lightgreen;
}
.spacing {
    Margin-right: 10px;
}
</style>