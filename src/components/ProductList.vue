<script lang="ts">
import {
    Vue,
    Component,
    Prop
} from 'vue-property-decorator';


@Component({
    components: {
        ProductItem: () => import('./ProductItem.vue'),
    },
})
export default class ProductList extends Vue {
    product: Object = {
    id: "1",
    name: " Quần sịp con voi chủ chốt ",
    price: "1.000.000đ"
}
}
</script>

<template>
<div class="danh-muc">
    <div class="product-list">
        <div class="container-fluid">
            <div class="title"> Quần lót nam </div>
            <div class="product-list-content">
                <ProductItem :product="product"/>
                <ProductItem :product="product"/>
                <ProductItem :product="product"/>
                <ProductItem :product="product"/>
            </div>
        </div>
    </div>
</div>
</template>


<style lang="less">
.container-fluid {
    max-width: 1110px;
    padding-right: 15px;
    padding-left: 15px;
    margin-right: auto;
    margin-left: auto;
}
</style>
