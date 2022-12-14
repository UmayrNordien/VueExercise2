<template>
  <div v-if="array">
    <div v-for="item in array" :key="item">

      <div class="container-fluid pt-5">
        <div class="row justify-content-evenly">
          <div class="card" style="width: 288px;">
            <img :src="item.image" class="card-img-top" alt="">
            <div class="card-body">
              <h4 class="card-title text-black">{{ item.name }}</h4>
              <p class="card-text text-black">In Stock: {{ item.quantity }}</p>
              <p class="card-text text-black">Price: {{ item.price }}</p>
              <a id='addCheckout' class="btn btn-light">🛒</a>
            </div>
          </div>
        </div>
      </div>

    </div>
  </div>
</template>


<script>
export default {
  data() {
    return {
      array: [
        {
          name: 'Graphic T',
          price: 800,
          image: 'https://i.postimg.cc/P56qnJ4S/Crew-Neck-1.jpg',
          quantity: 1
        },

        {
          name: ' Graphic Sweat-Shirt',
          price: 1000,
          image: 'https://i.postimg.cc/L8tD8d7Y/Graphic-Sweat-Shirt-1.jpg',
          quantity: 3
        },

        {
          name: 'Carhartt Bones Jacket',
          price: 2200,
          image: 'https://i.postimg.cc/1XzWTW5C/Carhartt-Bones-1.jpg',
          quantity: 2
        },

        {
          name: 'Graphic SW Pants',
          price: 1800,
          image: 'https://i.postimg.cc/cCfd6Mnc/275834450-542228100497493-5314424466359396574-n.jpg',
          quantity: 4
        }
      ]
    }
  }
};

// addCheckout() {
//       alert(`${'Item added to checkout'}`)
// };
</script>