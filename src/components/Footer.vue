<template>
<div class="footer">
    <div class="footer-top">
        <div class="container-fluid">
            <div class="ant-row" style="margin-left: -8px; margin-right: -8px;">
                <div class="gutter-row ant-col ant-col-6" style="padding-left: 8px; padding-right: 8px;">
                    <div class="footer-logo"><a href="/" class="router-link-active"><img src="https://sipconvoi.com/img/logo.654be934.png"></a></div>
                </div>
                <div class="gutter-row ant-col ant-col-6" style="padding-left: 8px; padding-right: 8px;">
                    <div class="title">HỖ TRỢ</div>
                    <div class="footer-item"><a href="#"> Trạng thái đơn hàng </a></div>
                    <div class="footer-item"><a href="#"> Hướng dẫn chọn size </a></div>
                    <div class="footer-item"><a href="#"> Hướng dẫn đặt hàng </a></div>
                    <div class="footer-item"><a href="#"> Câu hỏi thường gặp </a></div>
                </div>
                <div class="gutter-row ant-col ant-col-6" style="padding-left: 8px; padding-right: 8px;">
                    <div class="title">GIỚI THIỆU</div>
                    <div class="footer-item"><a href="#"> Trạng thái đơn hàng </a></div>
                    <div class="footer-item"><a href="#"> Hướng dẫn chọn size </a></div>
                    <div class="footer-item"><a href="#"> Hệ thống cửa hàng </a></div>
                    <div class="footer-item"><a href="/blog"> Blog </a></div>
                </div>
                <div class="gutter-row ant-col ant-col-6" style="padding-left: 8px; padding-right: 8px;">
                    <div class="title">CHÍNH SÁCH BÁN HÀNG</div>
                    <div class="footer-item"><a href="#"> Chính sách đổi trả </a></div>
                    <div class="footer-item"><a href="#"> Chính sách vận chuyển </a></div>
                    <div class="footer-item"><a href="#"> Chính sách thanh toán </a></div>
                    <div class="footer-item"><a href="#"> Chính sách bảo mật </a></div>
                </div>
            </div>
        </div>
    </div>
    <div class="footer-bottom"> © 2021 <a href="/" class="router-link-active">SipConVoi</a>. All rights reserved. </div>
</div>
</template>

<script lang="ts">
import {
    Component,
    Prop,
    Vue
} from "vue-property-decorator";

@Component
export default class Footer extends Vue {
    @Prop() private msg!: string;
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->

<style lang="less" scoped>
.footer {
    padding-top: 20px;
    background-color: #f2f2f2
}

.footer-logo {
    width: 70%;
    height: 100%
}

.footer-logo img {
    width: 100%
}

.footer .title {
    font-size: 18px;
    font-weight: 700;
    margin-bottom: 20px
}

.footer-item {
    padding: 6px 0;
    font-size: 14px
}

.footer-top {
    padding-bottom: 20px
}

.footer-bottom {
    border-top: 2px solid #1890ff;
    padding: 4px;
    background-color: #fff;
    text-align: center;
    font-size: 14px;
    height: 40px;
    line-height: 37px
}

.footer-bottom a {
    color: #1890ff
}

.container-fluid {
    margin: 0 110px;
}

a {
    color: #000;
}
</style>
