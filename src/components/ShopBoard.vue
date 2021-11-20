<template>
    <div>
      <navbar ref="navbar"></navbar>
      <alert></alert>
        
        <router-view ></router-view>
      <shopFooter ref="footer"></shopFooter>
    </div>
</template>

<script>
import Navbar from './ShopNavbar.vue';
import Alert from './AlertMessage.vue';
import ShopFooter from './Footer.vue';
    export default {
      components:{
        Navbar,
        Alert,
        ShopFooter,
      },
      created(){
        var headers = {};
        const token = document.cookie.replace(/(?:(?:^|.*;\s*)hexToken\s*=\s*([^;]*).*$)|^.*$/, '$1');
        this.$http.defaults.headers.common.Authorization = `${token}`;
        // this.$http.defaults.headers= headers;
    },
    methods:    {
        updateItme(){
  console.log('updateItme父')
            this.$refs.navbar.getUser()
            return 
        }
    },
        
    }
</script>

<style lang="scss" scoped>

</style>