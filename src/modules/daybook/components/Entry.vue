<template>
	<div
		class="entry-container mb-3 pointer p-2"
		@click="$router.push({ name: 'entry', params: { id: 10 } })"
	>
		<div class="entry-title d-flex">
			<span class="text-success fs-5 fw-bold">25</span>
			<spa class="mx-1 fs-5">Abril</spa>
			<spa class="mx-2 fw-light">2023, Martes</spa>
		</div>

		<div class="entry-description">
			<p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Cum iure ullam at facere nulla, suscipit alias rem placeat velit fuga dolore ipsa commodi expedita eaque omnis, ex non excepturi iusto?</p>
		</div>
	</div>
</template>
<script>
export default {};
</script>

<style lang="scss" scoped>
.entry-container {
	border-bottom: 1px solid #2c3e50;
	transition: 0.2s all ease-in;
	margin-bottom: 0 !important;

	&:hover {
		background-color: lighten($color: rgb(113, 155, 158), $amount: 40);
		transition: 0.2s all ease-in;
	}

	.entry-description {
		margin: 0;
		padding: 7px;
		font-size: 12px;
	}
}
</style>
