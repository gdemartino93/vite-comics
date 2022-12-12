<script >
export default{
  data(){
    return{
             dcComics : ["Characters", "Comics", "Movies", "TV"],
             Shop : ["Shop DC", "Shop DC Collectibles"],
             DC : ["Terms of Use", "Privacy Policy(New)", "Ad Choices", "Advertising"],
             Sites : ["dc", "Mad Magazine", "DC Kids"]
          
        // footerLinks : [
        //     {
        //         dcComics : ["Characters", "Comics", "Movies", "TV"],
        //         Shop : ["Shop DC", "Shop DC Collectibles"],
        //         DC : ["Terms of Use", "Privacy Policy(New)", "Ad Choices", "Advertising"],
        //         Sites : ["dc", "Mad Magazine", "DC Kids"]
        //     }
        // ]
    }
  }
}

</script>

<template>
 <section class="footerlink">
    <div class="container">
        <div class="link">
            <ul >
                <span>DC COMICS</span>
                <li v-for="(title,index) in dcComics" :key="index">
                    <a href="">{{title}}</a>
                </li>
            </ul>
            <ul >
                <span>DC</span>
                <li v-for="(title,index) in DC" :key="index">
                    <a href="">{{title}}</a>
                </li>
            </ul>
            <ul >
                <span>SITES</span>
                <li v-for="(title,index) in Sites" :key="index">
                    <a href="">{{title}}</a>
                </li>
            </ul>
            <ul >
                <span>SHOP</span>
                <li v-for="(title,index) in Shop" :key="index">
                    <a href="">{{title}}</a>
                </li>
            </ul>
        </div>
        <!-- img da fixare -->
        <!-- <img src="../../public/dc-logo-bg.png" alt=""> -->
        
        
    </div>
    
 </section>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
.link{
    display: flex;
    gap: 30px;
    width: 40%;
    flex-wrap: wrap;
}
.container{
    max-width: 1300px;
    margin: 0 auto;
    padding: 30px 0;
}
.footerlink{
   
    background-image: url(../../public/footer-bg.jpg);
    ul{
        color: white;
        font-weight: bold;
        font-size: 25px;
        li{
            list-style: none;
            font-size: 15px;
            margin: 15px 0;
            a{
                color: grey;
            }
        }
    }
}


</style>
