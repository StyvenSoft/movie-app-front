<template>
  <div class="home">
    <div class="featured-card">
      <router-link to="/movie/tt0409591">
        <img
          src="https://www.atomcreativemedia.com/wp-content/uploads/2018/09/orange-and-blue-movies-2.jpg"
          alt="Font poster"
          class="featured-img"
        />
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

    <form @submit.prevent="" class="search-box">
      <input type="text" placeholder="What are you looking for?" />
      <input type="submit" value="Search" />
    </form>

    <div class="movie-list">MOVIES</div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
.home {
  .featured-card {
    position: relative;

    .featured-img {
      display: block;
      width: 100%;
      height: 300px;
      object-fit: cover;

      position: relative;
      z-index: 0;
    }

    .detail {
      position: absolute;
      left: 0;
      right: 0;
      bottom: 0;
      background-color: rgb(0, 0, 0, 0.6);
      padding: 16px;
      z-index: 1;

      h3 {
        color: #fff;
        margin-bottom: 16px;
      }

      p {
        color: #fff;
      }
    }
  }

  .search-box {
    display: flex;
    flex-direction: column;
    justify-content: center;
    padding: 16px;

    input {
      display: block;
      appearance: none;
      border: none;
      outline: none;
      background: none;

      &[type="text"] {
        width: 100%;
        color: #fff;
        background-color: #496583;
        font-size: 20px;
        padding: 10px 16px;
        border-radius: 8px;
        margin-bottom: 15px;
        transition: 0.4s;

        &::placeholder {
          color: #f3f3f3;
        }

        &:focus {
          box-shadow: 0 3px 6px rgb(0, 0, 0, 0.2);
        }
      }

      &[type="submit"] {
        width: 100%;
        min-width: 300px;
        background-color: #42b883;
        padding: 16px;
        border-radius: 8px;
        color: #fff;
        font-size: 20px;
        text-transform: uppercase;
        transition: 0.4s;

        &:active{
          background-color: #3b8070;
        }
      }
    }
  }
}
</style>