<template>
  <div class="home">
    <div class="featured-card">
      <router-link to="/movie/tt0409591">
        <img src="https://www.atomcreativemedia.com/wp-content/uploads/2018/09/orange-and-blue-movies-2.jpg" alt="Font poster" class="featured-img" />
        <dic class="detail">
          <h3>More movies</h3>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Eligendi
            voluptatibus, omnis est perferendis earum vero atque ex eius,
            officia facilis veniam, ad architecto. Nihil ea expedita maiores
            dolores tempora quia!
          </p>
        </dic>
      </router-link>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
.home{
  .featured-card{
    position: relative;

    .featured-img{
      display: block;
      width: 100%;
      height: 300px;
      object-fit: cover;

      position: relative;
      z-index: 0;
    }

    .detail{
      position: absolute;
      left: 0;
      right: 0;
      bottom: 0;
      background-color: rgb(0, 0, 0, 0.6);
      padding: 16px;
      z-index: 1;

      h3{
        color: #fff;
        margin-bottom: 16px;
      }

      p{
        color: #fff;

      }
    }
  }
}
</style>