<template>
<div class="ui container">
	<div v-for="billet in billets">
		<div class="ui grid">
			<div class="two wide column icon-title">
				<img class="ui mini circular image" style="margin: 0" src="http://semantic-ui.com/images/logo.png">
			</div>
			<div class="ten wide column">
				<h2>{{ billet.titre }}</h2>
			</div>

			<div class="four wide column right aligned">	    
				<a class="ui teal tag label">Featured</a>
			</div>
		</div>

		<div class="ui divider"></div>

	    <p>{{ billet.resume }}</p>
		
		<div class="ui grid">
			<div class="eight wide column">
			    <p class="post-date">Posté le 25 décembre 2301</p>
		    </div>
			<div class="eight wide column right aligned">
			    <a href="#">Lire la suite..</a>
		    </div>	    
		</div>

        <div class="ui horizontal divider">
		   FIN D'ARTICLE
		</div>
	</div>

	<div class="paginate">
		<div class="ui pagination menu">
			<a class="item">
				1
			</a>
			<div class="item">
				2
			</div>
			<a class="item">
				3
			</a>
			<a class="item">
				4
			</a>
			<a class="item">
				5	
			</a>
		</div>
	</div>

</div>
</template>

<script>
export default {
	data: function() {
		return {
			billets: [
				{titre: "Nouvelle technologie REVOLUTIONNAIRE", resume: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum."},
				{titre: "INCROYABLE découverte de la NASA", resume: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum."},
				{titre: "Nouvelle série en réalité AUGMENTEE", resume: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum."},
			]
		}
	}
}
</script>

<style scoped>
	.ui.container{
		width: 40%;
	}
	.ui.horizontal.divider{
		margin: 10px 0 50px 0;
	}
	.post-date{
		font-style: italic;
		color: grey;
		font-size: 12px;
	}
	.paginate{
		text-align: right;
		margin-bottom: 50px;
	}
	.two.wide.column.icon-title{
		width: 8%;
		padding: 0 auto;
		margin: 0;
	}
</style>
