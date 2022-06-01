<template>
    <div>  
        <div class="mail-input d-flex">
            <input type="text" placeholder="Insert your mail ...">
            <div class="ms-btn d-flex align-items-center mx-3"> 
                Subscribe
            </div>
        </div>
        <p class="mt-3">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Ipsam, dolor</p>
    </div>
</template>

<script>
export default {
    name: "MyMailingList",
}
</script>

<style lang="scss" scoped>
@import "../style/common.scss";

input {
    border-radius: 15px;
    border: none;
    width: 400px;
    font-size: .8em;
    padding-left: 15px;
}

p {
    color: $jumbo;
}
</style>
