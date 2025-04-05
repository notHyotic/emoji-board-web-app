<script setup lang="ts">
const props = defineProps<{
	emojiName: string
	imgUrl: string
}>()

const emojiHeight = "60px"

// Function to copy the image URL to the clipboard
const copyImageToClipboard = async () => {
	await navigator.clipboard.writeText(props.imgUrl)
}
</script>

<template>
	<div
		class="rounded-2xl border-2 border-solid border-black bg-amber-200"
		@click="copyImageToClipboard"
	>
		<div class="m-2 flex flex-col">
			<img class="" :src="imgUrl" :height="emojiSize" :width="emojiHeight" />
			<div class="text-center font-bold">
				{{ emojiName }}
			</div>
		</div>
	</div>
</template>
