<template>
    <div class="mt-5">
        <v-row
            v-for="(product,i) in $store.state.products"
            :key="i"
        >
            <HorizontalProduct
                :product="product"
                btnAction="remove"
            />
        </v-row>
    </div>
</template>
<script>
import HorizontalProduct from '../cards/HorizontalProduct.vue'
export default {
    components:{
        HorizontalProduct
    },
    methods:{
        removeFromCart(){}
    }
}
</script>