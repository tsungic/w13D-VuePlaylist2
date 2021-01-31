<template>
    <div>
        <listSong v-for=" song in songs " :key=song.title :song= "song" :isInplayList= " false " />
    </div>
</template>

<script>
import listSong from "./song";
    export default {
        name: "songsList",
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