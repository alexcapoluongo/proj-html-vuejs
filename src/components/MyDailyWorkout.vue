<template>
    <div class="daily d-flex justify-content-center align-items-center">
        <div class="text-center">
            <!-- bottone play -->
            <div class="play-btn m-auto">
                <i class="fas fa-play"></i>
            </div>
            <h1>Crossfit workout of the day</h1>
            <h3>November 15th, 2019</h3>
            <a href="">View all videos --></a>
        </div>
    </div>
</template>

<script>
export default {
    name: "MyDailyWorkout",
}
</script>

<style lang="scss" scoped>
@import "../style/common.scss";

.daily {
    height: 100%;
    width: 100%;
    background: rgb(0, 0, 0);
    background: linear-gradient(150deg, rgba(3, 13, 151, 0.777) 10%, rgba(117, 1, 1, 0.782) 100%);
}

.play-btn {
    background-color: white;
    display: flex;
    justify-content: center;
    align-items: center;
    border-radius: 50%;
    height: 55px;
    width: 55px;

        i {
            color: $dodgerblue;
            font-size: .8em;
        }
    }

h3 {
    color: yellow;
}

a {
    color: white;
}
</style>