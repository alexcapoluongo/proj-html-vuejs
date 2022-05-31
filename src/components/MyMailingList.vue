<template>
<div>  
    <div class="mail-input d-flex">
        <input type="text" placeholder="Insert your mail ...">
        <button class="ms-btn mx-3"> Subscribe </button>
    </div>
    <p class="mt-3">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Ipsam, dolor</p>

</div>

</template>

<script>
export default {
    name: "MyMailingList",
    data() {
        return {
            //maybe a props????
        }
    }
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

.ms-btn {
    white-space: nowrap; 
    color:white;
    border: none;
    background-color: #4154fe;
    border-radius: 15px;
    width: auto;
    height: 35px;      
    padding: 15px;      
    padding-left: 50px;
    padding-right: 50px;
    font-size: .7em;
    
    &:hover {
        background-color: #ec5a57;
    }
}

p {
    color: $jumbo;
}
</style>
