<template>
    <!-- Section: Design Block -->
    <section class="mb-32 text-gray-800 background-radial-gradient">
      <div class="px-6 py-12 md:px-12 text-center lg:text-left">
        <div class="container mx-auto">
          <div class="grid lg:grid-cols-2 gap-12 flex items-center">
            <div class="mt-12 lg:mt-0">
              <h1 class="text-5xl md:text-6xl xl:text-7xl font-bold tracking-tight mb-12"
                style="color: hsl(218, 81%, 95%)">
                Are you ready <br /><span style="color: hsl(218, 81%, 75%)">for the big sale?</span>
              </h1>
              <p class="text-lg" style="color: hsl(218, 81%, 95%)">
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Minima officia consequatur
                adipisci tenetur repudiandae rerum quos.
              </p>
            </div>
            <div class="mb-12 lg:mb-0">
              <img src="~/assets/images/shopping-icons.png">
            </div>
          </div>
        </div>
      </div>
    </section>
    <!-- Section: Design Block -->
</template>

<script setup>

</script>

<style scoped>
 h2 {
    margin-bottom: 30px;
    font-size: 36px;
 }
 p {
    margin: 20px 0;
 }

 .background-radial-gradient {
          background-color: hsl(218, 41%, 15%);
          background-image: radial-gradient(650px circle at 0% 0%,
              hsl(218, 41%, 35%) 15%,
              hsl(218, 41%, 30%) 35%,
              hsl(218, 41%, 20%) 75%,
              hsl(218, 41%, 19%) 80%,
              transparent 100%),
            radial-gradient(1250px circle at 100% 100%,
              hsl(218, 41%, 45%) 15%,
              hsl(218, 41%, 30%) 35%,
              hsl(218, 41%, 20%) 75%,
              hsl(218, 41%, 19%) 80%,
              transparent 100%);
        }
</style>