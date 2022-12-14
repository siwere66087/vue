<template>
    <h2>products</h2>
    <div class="cards">
<Product></Product>
    </div>
</template>

<script>
   import Product from '@/components/product.vue';
   export default{
    name:'myproduct',
    components:{ Product }
   }
</script>

