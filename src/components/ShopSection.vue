<template>
    <div>

        <section
        class="jumbotron text-center"
        style="
          background-size: cover;
          background-position: center;
          background-image: url('http://localhost:8082/16348130439051457.jpg');
        "
        :style="{ backgroundImage: `url(${imageUrl})` }"
      >
        <div class="container">
          <div class="row justify-content-center align-items-center">
            <div class="col-4">
              <h1 class="display-4 t-shadow">娃娃世界</h1>
              <p class="lead">各種可愛的娃娃，在這都可以找的到</p>
              <p class="lead">台北市信義區XXX路XXX號</p>
            </div>
          </div>
        </div>
      </section>

    </div>
</template>

<script>
    export default {
        
    }
</script>

<style lang="scss" scoped>

</style>