<template>
	<div class="container">
		<p> {{ msg }}</p>
		<p v-html="htmlString" ></p>
		<div v-show="show">
			elemento exibido aki
		</div>
		<img width="150" :src="'/assets/img/' + fileName" />
		<div v-bind="{ id: idVar, 'data-item': dataItem }">elemento</div>

	</div>
</template>

<script>

	export default {
		name: 'Diretivas',	
		data() {
			return {
				msg: 'texto raw',
				htmlString: '<strong>texto negrito</strong>',
				show: true,
				fileName: 'vue.jpg',
				idVar : 'id-01',
				dataItem : 'nome',
				
			}
		},
	}
</script>

