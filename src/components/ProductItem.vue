<template>
<div class="product-item">
    <a href="/ProductDetail" class="product-item-image">
        <div class="box-see"> XEM NGAY </div>
        <img src="https://i.imgur.com/r5LZRFr.jpg" alt="Quần sịp con voi chủ chốt - sipconvoi.com" title="Quần sịp con voi chủ chốt - sipconvoi.com">
    </a>
    <div class="product-item-details">
        <div class="product-item-name">
            <a href="/ProductDetail" class="">Quần sịp con voi chủ chốt</a>
        </div>
        <div class="product-item-price"> 1.000.000đ</div>
        <div class="product-item-price">{{product.price}}</div>
        <div class="product-item-code"> S-VOI1 </div>
    </div>  
</div>
</template>

<script lang="ts">
import {
    Component,
    Prop,
    Vue
} from "vue-property-decorator";

@Component
export default class ProductItem extends Vue {
    @Prop() product: any;
}
</script>

<style lang="less" scoped>
.container-fluid {
    max-width: 1110px;
    padding-right: 15px;
    padding-left: 15px;
    margin-right: auto;
    margin-left: auto;
}

.product-item {
    padding: 6px;
    display: inline-block;
    cursor: pointer;
    -webkit-user-select: none;
    -moz-user-select: none;
    -ms-user-select: none;
    user-select: none
}

.product-item-image {
    display: block;
    position: relative;
    width: 100%;
    height: 250px;
    background-color: #fff;
    overflow: hidden
}

.product-item-image .box-see {
    position: absolute;
    width: 100%;
    height: 35px;
    line-height: 35px;
    background-color: #668eca;
    color: #fff;
    bottom: -35px;
    text-align: center;
    font-size: 16px;
    cursor: pointer;
    transition: all .3s
}

.product-item-image:hover .box-see {
    bottom: 0
}

.product-item-image img {
    width: 100%
}

.product-item-details {
    padding-top: 12px;
    padding-bottom: 12px
}

.product-item-name {
    font-size: 16px;
    margin-bottom: 8px
}

.product-item-name a:hover {
    text-decoration: underline;
    color: inherit
}

.product-item-price {
    font-size: 22px;
    font-weight: 700
}

.product-item-code {
    margin-top: 4px;
    font-size: 12px
}

.product-list {
    background-color: #f2f2f2;
    padding: 25px 0
}

.product-list-content {
    display: block
}

.product-list .title {
    text-align: center;
    font-size: 34px
}

.product-list .product-item {
    width: 25%;
    margin-top: 40px;
    padding-left: 12px;
    padding-right: 12px
}

.product-list .product-item:first-child {
    padding-left: 0;
    padding-right: 12px
}

.product-list .product-item:last-child {
    padding-left: 12px;
    padding-right: 0
}
</style>
