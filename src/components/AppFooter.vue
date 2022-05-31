<template>
  
<footer class="footer">
    <div class="ms-container">
        <div class="footer_top d-flex justify-content-between">
            <ul>
                <li class="image">
                    <img src="" alt="" srcset="">
                </li>
                <li></li>
                <li>
                    <ul>
                        <li class="socials"></li>
                    </ul>
                </li>
            </ul>
            <ul>
                <li></li>
            </ul>
            <ul>
                <li></li>
            </ul>
        </div>
        <div class="footer_bottom"></div>
    </div>
</footer>

</template>

<script>
export default {
    name: "AppFooter"
}
</script>

<style lang="scss" scoped>
@import "../style/common.scss";

.footer {
    height: 500px;
    background-color: #0d0b12;
    color: white;

    &_top {
        ul {
            border: 1px solid white;
            width: 30%;
        }
    }
}

</style>