<script lang="ts">
    import { onMount } from 'svelte';
    import YouTubePlayer from 'youtube-player';
    onMount(async () => {
        let firstStateChange;

        let player1 = YouTubePlayer('player-1', {
            playerVars:{
            }
        });
        await player1.playVideo()
        // await player1.loadPlaylist('PLMoZgWjm14OF2AWFfPc3cyQH7T2SC89jo');
    })
</script>

<div id='player-1'></div>