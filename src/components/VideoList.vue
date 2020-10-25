<template>
    <ul class="list-group">
        <VideoListItem 
        :key="video.etag"
        v-for="video in videos"
        :video="video"
        
        >
        </VideoListItem>
    </ul>
    
</template>

<script>
import VideoListItem from './VideoListItem';



export default {
    name: 'Videolist',
    components: {
        VideoListItem
    },
    props: ['videos']
}
</script>

<style>

</style>