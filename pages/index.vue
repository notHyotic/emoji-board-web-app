<script setup lang="ts">
import logoUrl from "~/assets/img/flushedbread.png"
</script>

<template>
	<div class="flex h-screen w-screen flex-row">
		<div id="sidebar" class="h-full w-[20%] bg-amber-600">
			<div
				id="app-banner"
				class="flex flex-col border-b-2 border-solid border-b-amber-300"
			>
				<div class="p-2 text-5xl font-extrabold text-amber-300">
					EMOJI BOARD
				</div>
				<div class="flex justify-center">
					<img :src="logoUrl" class="h-[80px] w-[80px]" />
				</div>
			</div>

			<div id="collections" class="space-y-1 border-b-2 border-b-amber-300 p-6">
				<div
					class="text-bamber-300 block pb-2 text-xs tracking-widest uppercase dark:text-amber-950"
				>
					Collections
				</div>

				<CollectionTitle title="Smileys & Emotion" />
			</div>
		</div>

		<div id="main-site" class="flex h-full w-[80%] flex-col bg-amber-100">
			<div class="items-center p-5">
				<Searchbar />
			</div>

			<div id="emoji-board" class="p-5">
				<Emoji
					imgUrl="https://cdn.discordapp.com/emojis/1143155561202974750.webp?size=128"
					emojiName="pistash"
				/>
			</div>
		</div>
	</div>
</template>
