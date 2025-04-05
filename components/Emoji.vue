<script setup lang="ts">
defineProps<{
	emojiName: string
	imgUrl: string
}>()

const emojiHeight = "60px"
</script>

<template>
	<div class="border-solid border-black border-2">
		<img :src="imgUrl" :height="emojiSize" :width="emojiHeight" />
		<div>
			{{ emojiName }}
		</div>
	</div>
</template>
