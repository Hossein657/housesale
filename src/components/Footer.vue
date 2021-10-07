<template>
    <footer>
        <div class="container">
            <ul>
                <li><router-link to="/OnSale">On sale</router-link></li>
                <li><router-link to="/ForRent">For rent</router-link></li>
                <li><router-link to="/About">About us</router-link></li>
                <li><router-link to="/News">Property news</router-link></li>
            </ul>
            
            <ul>
                <li class="logo"><router-link to="/"><img src="../assets/logo.png" alt=""></router-link></li>
                <li><p>© 2020 Housesale Technologies Ltd.</p></li>
                <li><p>1760  Dancing Dove Lane, New York, USA</p></li>
                <li><a href="mailto: sales@housesales.com" target="_blank">sales@housesales.com</a></li>
            </ul>
        </div>
    </footer>
</template>

<script>
export default {
    name: "Navbar"
}
</script>

<style scoped>
    footer{
        background-color: #093A7A;
    }
    a, p{
        color: #fff;
    }
    ul{
        display: flex;
        align-items: center;
    }
    ul:first-child{
        border-bottom: 1px solid #10458a;
    }
    li{
        margin: 40px;
    }

</style>