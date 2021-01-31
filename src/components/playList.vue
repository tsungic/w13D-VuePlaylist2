<template>
    <div>
        <listSong v-for=" song in songs " :key=song.title :song= "song" :isInplayList= "true" />

    </div>
</template>

<script>
import listSong from "./song";
    export default {
        name: "playList",
        components:{
            listSong
        },
        props : {
            songs : {
                type : Array,
                required : true
            }
        }
    }
    
</script>

<style scoped>

</style>