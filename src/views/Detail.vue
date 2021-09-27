<template>
  <div class="detail-page">
    <div class="container">
        <img src="https://i.imgur.com/Cxxf5A4.jpg" alt="">
        <div class="product-detail">
            <div class="title">Quần sịp nam lưới - S-L1</div>
            <div class="ma-sp">
                Mã SP: S-L1
            </div>
            <div class="price">
                499.999đ
            </div>
            <div class="size-title">Size:</div>
            <div class="size"><span>S</span><span>M</span><span>L</span><span>XL</span><span>XXL</span></div>
            <button class="add-cart">THÊM VÀO GIỎ</button>
        </div>
    </div>
  </div>
</template>
<style lang="css">
    .detail-page {
        display: flex;
        text-align: left;
        font-family: 'Roboto', sans-serif;
        padding: 50px 0;
    }
    .container {
        margin: auto;
        width: 80%;
        display: flex;
    }
    .product-detail {
        flex: 1;
        padding-left: 30px;
    }
    .title {
        font-size: 30px;
        margin: 3.5px 0 7px;
    }
    .ma-sp {
        display: block;
        color: #707070;
        font-weight: 700;
        margin-bottom: 8px;
    }
    .price {
        color: #a0122b;
        font-size: 26px;
        font-weight: 700;
        display: inline-block;
        margin-bottom: 8px;
    }
    .size-title {
        font-weight: 500;
        margin: 0 0 10px;
        padding: 3.5px 0;
        font-size: 15.4px;
        color: rgba(0,0,0,.7);
    }
    .size span {
        min-width: 56px;
        height: 42px;
        line-height: 42px;
        cursor: pointer;
        align-items: center;
        justify-content: center;
        display: inline-flex;
        border: 1px solid #ccc;
        background: #fff;
        margin: 0;
        position: relative;
        font-size: 15px;
        font-weight: 600;
        margin: 0 7px 3.5px 0;
    }
    .size span:hover {
        background: rgba(0,0,0,.07);
    }
    .add-cart {
        max-width: 250px;
        width: 100%;
        display: block;
        padding: 0;
        border: 0;
        font-weight: 600;
        background: #007aff;
        font-size: 14px;
        text-transform: uppercase;
        color: #fff;
        line-height: 36px;
        text-align: center;
        letter-spacing: 2px;
        border-radius: 3px;
        border: 2px solid #007aff;
        margin-top: 20px;
    }
</style>
