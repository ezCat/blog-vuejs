<template>
	<div class="ui container">
		<h2>Ajouter un article</h2>
		<div class="ui divider" style="margin-bottom: 50px;"></div>

		<div class="ui form">
			<div class="field">
			    <label>Titre</label>
				<div class="ui input">
				  <input type="text" placeholder="Titre de l'article" v-model="titre">
				</div>
			</div>
			<div class="field">
				<label>Contenu</label>
				<textarea placeholder="Contenu de l'article" v-model="contenu"></textarea>
			</div>
		</div>
		<div class="field">
			<br>
			<button class="ui button teal" type="submit" v-on:click="addBillet">Poster</button>
		</div>

		<div v-for="billet in billets" transition="expand">
			<h2>{{ billet.titre }}</h2>
			<p> {{ billet.contenu }} </p>
		</div>
	</div>
</template>

<script>
export default{
	data: function() {
		return {
		  billets: []
		}
	},
	methods: {
		addBillet: function() {
			this.billets.push({titre: this.titre, contenu: this.contenu})
			this.titre = ''
			this.contenu = ''
		}
	}
}
</script>

<style scoped>
	
</style>