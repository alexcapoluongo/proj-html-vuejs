<template>
  
<footer class="footer">
    <div class="ms-container d-flex align-items-center">
        <div class="footer_top d-flex justify-content-between text-center">
            <ul>
                <li class="image mb-3">
                    <img src="../assets/img/logo.png" alt="" srcset="">
                </li>
                <li class="mb-5">
                    <p >Lorem ipsum dolor, sit amet consectetur adipisicing elit. Mollitia hic veniam sit, consectetur repellat nesciunt quisquam optio ratione a obcaecati numquam ipsa cumque. Tenetur neque corporis culpa voluptatibus, provident at.</p>
                </li>
                <li>
                    <ul class="socials d-flex justify-content-between m-auto">
                        <li><i class="fa-brands fa-facebook-f"></i></li>
                        <li><i class="fa-brands fa-twitter"></i></li>
                        <li><i class="fa-brands fa-youtube"></i></li>
                        <li><i class="fa-brands fa-instagram"></i></li>
                        <li><i class="fa-brands fa-linkedin"></i></li>
                    </ul>
                </li>
            </ul>
            <ul class="recent-post">
                <li>
                    <h6>RECENT POSTS</h6>
                </li>
                <li v-for="(item, idx) in listArray" :key="idx">> {{ item }}</li>
            </ul>
            <ul>
                <li>
                    <h6 class="mb-4">CONTACT INFORMATION</h6>
                </li>
                <li class="contact-list" v-for="(item, idx) in contactObject" :key="idx">
                    <p class="text-secondary mb-5">{{ item.address }}</p>
                    <p>Mobile: {{ item.mobile }}</p>
                    <p>Email: {{ item.email }}</p>
                </li>
            </ul>
        </div>
    </div>
    <div class="footer_bottom">
        <div class="ms-container">
            <p class="text-secondary text-center"> &copy; Copyright 2012- 2020 | Acada theme by <span>ThemeFusion</span> | All rights reserved | Powered by <span>WordPress</span></p>
        </div>
    </div>
</footer>

</template>

<script>
export default {
    name: "AppFooter",
    data() {
        return {
            listArray: [
                'The best protein shake',
                'Ultimate cardio workout', 
                'New juices available now', 
                'Tips to find training partners', 
                '20 best healthy recipes'
            ],

            contactObject: [
                {
                    address: "4746 Tipple Road Michigan 48449",
                    mobile: "1.800.000.0000",
                    email: "info@your-company.com"
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../style/common.scss";

.footer {
    height: 400px;
    background-color: #0d0b12;
    color: white;

    &_top {
        .recent-post {
            line-height: 3em;
        }

        .contact-list {
            line-height: 0;    
        }

        ul {
            border: 1px solid white;
            font-size: .8em;
            width: 30%;

            img {
                width: 60%;
            }

            .socials {
                width: 60%;      
                color: $monza;
                font-size:1.5em
            }
        }
    }

    &_bottom {
        height: 80px;
        line-height: 80px;
        background-color: #0d0b12;
        border-top: .5px solid $jumbo;

        span {
            color: white;
        }
    }
}

</style>