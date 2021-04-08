<template>
    <li>
       <div class="listSong">
            <img :src="img" alt="..." width="100" height="100">
            <div>
                <h1>{{name}}</h1>
            <small>{{singer}}</small>
            </div>
       </div>
    </li>
</template>
<script>
export default {
    props:['name','img','singer']
}
</script>
<style scoped>
li{
    list-style-type: none;
    padding:0;
    margin-top:15px;
}
.listSong img{
    border-radius: 20px;
}
.listSong{
    display: flex;
}
</style>