<template>
    <div v-if="array">
        <div v-for="item in array" :key="item">
            <div>
                <div class="container">
                    <div style="display: grid ; grid-template-columns: repeat(4, 1fr)">
                        <div class="card" style="width: 20rem; grid-column:span 1;">
                            <img :src="item.image" class="card-img-top" alt="">
                            <div class="card-body">
                                <h6 class="card-title">{{ item.name }}</h6>
                                <p class="card-text">{{ item.price }}</p>
                                <p class="card-text">{{ item.quantity }}</p>
                                <a href="#" class="btn btn-light">Add to cart</a>
                            </div>
                        </div>
                    </div>
                </div>

            </div>
        </div>
    </div>
</template>

<!-- <div class="card" style="width: 18rem;">
    <img class="card-img-top" src={{item.image}} alt="">
    <div class="card-body">
        <h5 class="card-title">{{ item.name }}</h5>
        <p class="card-text">{{ item.price }}</p>
        <a href="#" class="btn btn-light">Add to cart</a>
    </div>
</div> -->

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
            name: 'Sweat-Shirt',
            price: 1000,
            image: 'https://i.postimg.cc/L8tD8d7Y/Graphic-Sweat-Shirt-1.jpg',
            quantity: 3
          },
  
          {
            name: 'Jacket',
            price: 2200,
            image: 'https://i.postimg.cc/1XzWTW5C/Carhartt-Bones-1.jpg',
            quantity: 2
          },
  
          {
            name: 'Pants',
            price: 1800,
            image: 'https://i.postimg.cc/cCfd6Mnc/275834450-542228100497493-5314424466359396574-n.jpg',
            quantity: 4
          }
        ]
      }
    }
  }
  </script>