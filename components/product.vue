<template>
    <div class="col-2">
        <div>
        <div class="card" v-for="item in myproduct" :key="item">
            <img :src="item.image"
            style="width: 30rem;margin-left:3rem"
            />
            <div class="card-body">
                <h5 class="card-title">{{ item.product }}</h5>
                <p class="card-text">{{ item.brand }}</p>
                <p class="price">{{ item.price }}</p>
                <button class="btn btn-primary">Add to checkout</button>
            </div>
        </div>
    </div>
    </div>
</template>

<script>


export default {
    data() {
        return {
            myproduct: [
                {
                    "id": 1,
                    "product": "Foundations",
                    "brand": "Fentybeauty",
                    "image": "https://i.postimg.cc/T3fvVqJ8/foundationsjpg-image-668x550.jpg",
                    "price": "R600,00"
                },
                {
                    "id": 2,
                    "product": "Concealers",
                    "brand": "Mac",
                    "image": "https://i.postimg.cc/prJqR8h8/IMG-0181.webp",
                    "price": "R400,00"
                },
                {
                    "id": 3,
                    "product": "Bronzers",
                    "brand": "Yardley",
                    "image": "https://i.postimg.cc/k578PZNj/YAR-F122282-BLANK-1.jpg",
                    "price": "R250,00"
                },
                {
                    "id": 4,
                    "product": "Highlighters",
                    "brand": "Rimmel",
                    "image": "https://i.postimg.cc/tJnpcqYL/THREE.jpg",
                    "price": "R180,00"
                },
            ],
        };
    }
}
  </script>

<style  scoped>
#cards{
    display: flex;
    background-color: blue;
}
</style>




