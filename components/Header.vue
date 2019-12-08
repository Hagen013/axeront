<template>
    <div class="header">
        <div class="header-top">
            <div class="content-area">
            </div>
        </div>
        <div class="content-area">
            <div class="header-middle">
                <div class="header-logo ft">
                    <a href="/">
                        ТОРГ<span class="mint">ОСВЕТ</span>
                    </a>
                </div>
                <div class="header-search ft">
                    <div class="input-box">
                        <input class="input" placeholder="ПОИСК">
                    </div>
                </div>
            </div>
        </div>
        <div class="header-bottom">
            <div class="content-area">
            </div>
        </div>
    </div>
</template>

<script>
export default {
    
}
</script>

<style>
.header {
    width: 100%;
}
.header-top {
    position: absolute;
    top: 0px;
    left: 0px;
    height: 40px;
    width: 100%;
    background: #000000;
    z-index: 100;
}
.header-middle {
    height: 120px;
    width: 100%;
    padding-top: 40px;
}
.header-bottom {
    height: 48px;
    width: 100%;
    border-top: 1px solid #dcdcdc;
    border-bottom: 1px solid #dcdcdc;
}
.input-box {
    height: 46px;
    width: 100%;
}
.header-search {
    padding: 17px 0px;
    width: 448px;
}
.header-logo {
    height: 100%;
    width: 235px;
    font-size: 30px;
    font-weight: 900;
    line-height: 80px;
    user-select: none;
}
</style>
