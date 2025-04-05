<script setup lang="ts">
const props = defineProps<{
	title: string
	emojiSVG: string
}>()
</script>

<template>
	<a
		href="/smileys-emotion"
		class="flex h-9 w-full items-center rounded-md px-3 py-2 text-amber-200 hover:bg-gray-200 dark:hover:bg-gray-800"
	>
		<span class="text-md whitespace-nowrap">{{ title }}</span>
	</a>
</template>
