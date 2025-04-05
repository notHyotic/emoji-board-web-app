<script setup lang="ts">
defineProps<{
	emojiName: string
	imgUrl: string
}>()

const emojiHeight = "60px"
</script>

<template>
	<div class="rounded-2xl border-2 border-solid border-black bg-amber-200">
		<div class="m-2 flex flex-col">
			<img class="" :src="imgUrl" :height="emojiSize" :width="emojiHeight" />
			<div class="text-center font-bold">
				{{ emojiName }}
			</div>
		</div>
	</div>
</template>
