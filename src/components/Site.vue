<template>
    <webview id="webview"
             :src="src"
             useragent="Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/78.0.3904.108 Safari/537.36"></webview>
</template>
<script>
	export default {
		props: {
			src: {
				type: String,
				default: 'https://www.github.com/'
			}
		}
	}
</script>
<style>
    #webview {
        display: inline-flex;
        position: fixed;
        left: 400px;
        top: 0;
        height: 600px;
        width: calc(100% - 400px);
    }
</style>
