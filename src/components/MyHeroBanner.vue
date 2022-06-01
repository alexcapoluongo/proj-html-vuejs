<template>
    <div>
        <p class="mt-2 mb-4">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Atque aperiam minus.</p>
        <ul>
            <li><a class="ms-btn" href="">
                <i class="fa-brands fa-youtube mx-2"></i>Visit my Youtube Channel</a>
            </li>
            <li class="mx-2"><a class="ms-btn" id="btn-gray" href="">Buy Avada today -> </a></li>
        </ul>

        <div class="play-btn">
            <i class="fas fa-play"></i>
        </div>
    </div>
</template>

<script>
export default {
    name: "MyHeroBanner",
}
</script>

<style lang="scss" scoped>
@import "../style/common.scss";

.ms-container {
    background: linear-gradient(90deg, rgba(0,0,0,1) 40%, rgba(0,0,0,0) 97%);
}

p {
    color: $jumbo;
}

ul {
    display: flex;
    justify-content:flex-start;
    list-style: none;
    padding-left: 0;

    li {
        border-radius: 15px;
        display: flex;
        align-items: center;

        a {
            display: flex;
            align-items: center;
        }
    }
        #btn-gray {
            background-color: black;
            color: $jumbo;
            border: 1px solid $jumbo;

            &:hover {
                background-color: white;
                color: black;
            }
        }
}

.play-btn {
    position: absolute;
    right:300px;
    top: 30%;
}

</style>