<template>
    <ul>
        <song-item v-for="song in songs" :key="song.id" :name="song.name" :img="song.img" :singer="song.singer"></song-item>
    </ul>
</template>
<script>
import songItem from '../../components/song/songItem.vue';
export default {
    components:{
        songItem
    },
    inject:['songs']
}
</script>
<style scoped>

</style>