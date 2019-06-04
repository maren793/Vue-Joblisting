<template>
  <div id="app">
   <router-view></router-view>
  </div>
</template>

<script>
// Set storage variables for username and password.
        (function() {
            localStorage.setItem('username', 'Maren');
            localStorage.setItem('password', '@4321');
        })();

export default {
  name: 'app'
}
</script>


