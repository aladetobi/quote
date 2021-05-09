<template>
    <div class="list">
        <ul>
            <li>
                <a href="">&#128187;</a>
            </li>
            <li>
                <a href="">&#10017;</a>
            </li>
            <li>
                <a href="">&#129505;</a>
            </li>
            <li>
                <a href="">&#127968;</a>
            </li>
            <li>
                <a href="">&#129505;</a>
            </li>
            <li class="line"></li>
           
        </ul>
        <div class="link">
            <a href="">oyedokunaladetobi@gmail.com</a>
        </div>
        
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style scoped>
li {
    list-style: none;
    margin-top: 10px;
    text-align: center;
}
a{
   color: black;
   font-size: 15px;
    text-decoration: none;
 }
 .list {
     position: fixed;
     bottom: 0;
     left: 40px;
 }
 .link {
     position: fixed;
     right: 40px;
     bottom: 100px;
     transform: rotate(90deg);
     /* text-orientation: upright; */
 }
 .link a {
     font-size: 13px;
     text-align: center;
     color: #ddd;
     display: block;
 }
 .line {
     margin-left: 10px;
     height: 50px;
     width: 1px;
     background-color: #ddd;
 }

</style>