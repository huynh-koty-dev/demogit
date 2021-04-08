<template>
  <div id="app">
    <list-song></list-song>
  </div>
</template>

<script>
import ListSong from './pages/mainSong/ListSong.vue'
export default {
  name: 'app',
  components:{
    
    ListSong
  },
  
  data(){
    return{
      songs:[
      {
        id:0,
        name:"chung ta cua hien tai",
        img:"https://kenh14cdn.com/203336854389633024/2020/12/16/photo-1-1608088706527625974240-16080929200002104649977.jpg",
        src:"./assets/songs/chungtacuahientai.mp3",
        singer:'Son Tung MTP'
      },
      {
        id:1,
        name:"thang dien",
        img:"https://i.ytimg.com/vi/HXkh7EOqcQ4/maxresdefault.jpg",
        src:"./assets/songs/thangdien.mp3",
        singer: 'Justatee'
      }
    ]
    }
  },
  provide(){
      return{
        songs: this.songs
      }
  },
}
</script>

<style>


</style>
