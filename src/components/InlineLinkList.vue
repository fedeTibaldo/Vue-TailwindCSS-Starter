<template>
	<ul>
		<li class="inline-block mx-2" v-for="link in links">
			<a v-if="typeof link == 'object'" v-bind:href="link.url" target="_blank">
				{{ link.text }}
			</a>
		</li>
	</ul>
</template>

<script>
export default {
	props: ['links']
}
</script>