<template>
	<div class="entry-title d-flex justify-content-between p-2">
		<div>
			<span class="text-success fs-3 fw-bold">25</span>
			<span class="mx-1 fs-3 fw-bold">Abril</span>
			<span class="mx-2 fs-5 fw-light">2023</span>
		</div>
		<div>
			<button class="btn btn-danger mx-2">
				Borrar <i class="fa fa-trash-alt"></i>
			</button>
			<button class="btn btn-primary">
				Subir foto <i class="fa fa-upload"></i>
			</button>
		</div>
	</div>

	<hr />

	<div class="d-flex flex-column px-3 h-75">
		<textarea placeholder="Que sucedió hoy?"></textarea>
	</div>

	<Fab :icon="`fa-save`" />

	<img
		src="https://img.freepik.com/free-vector/mountains-landscape-sundown_52683-24164.jpg?w=1060&t=st=1682481618~exp=1682482218~hmac=ea8c869d78b7e8d2be23f593ba758b17d4920a2ae457b92b08d8ede658071b53"
		alt="entry-picture"
		class="img-thumbnail"
	/>
</template>
<script>
import { defineAsyncComponent } from 'vue';
export default {
	components: {
		Fab: defineAsyncComponent(() => import('../components/Fab.vue')),
	},
};
</script>
<style lang="scss" scoped>
textarea {
	font-size: 20px;
	border: none;
	height: 100%;
	resize: none;

	&:focus {
		outline: none;
	}
}

img {
	width: 200px;
	position: fixed;
	bottom: 150px;
	right: 20px;
	box-shadow: 0px 5px 10px rgba($color: #000000, $alpha: 0.2);
}
</style>
