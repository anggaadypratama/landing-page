<script>
	export let segment;
</script>

<style lang="scss">
	@import '../../static/style/global.scss';

	a{
		text-decoration: none;
	}

	.active{
		color: $secondary;
	}

	.sidebar {
		width: 60px;
		background-color: $primary-dark;
		color: $icon-off;
		font-family: $viga;
		position: fixed;
		display: flex;
		flex-direction: column;
		justify-content: space-between;
		min-height: 100%;
		margin: 0;
		padding: 0;

		

		.logo{
			width: 100%;
			height: 70px;
			background-color: $secondary;
			color: $primary;
			text-align: center;
		}

		nav {
			display: block;
			text-align: center;

			a{
				height: 50px;
				display: block;
				line-height: 50px;
				margin-bottom: 15px;
				position: relative;
			}
		}

		@media screen and (max-width: $md) {
			flex-direction: row;
			position: absolute;
			height: 50px;
			width: 100%;
			top: 0;
			left: 0;
			min-height: 0;
			
			.logo{
				width: 70px;
				height: 50px;
			}

			nav{
				width: 42%;
				position: absolute;
				left: 30%;
				float: left;
				display: flex;
				justify-content: space-evenly;
				height: 60px;
				top: 0;
				margin-top: 0;

				a{
					display: inline;

					&:first-child{
						margin-left: 0;
					}
				}
			}
		}
	}
</style>

<div class="sidebar">
	<a class="logo" href=".">Angga</a>
	<nav class="menu">
		<a aria-current='{segment === undefined ? "page" : undefined}' class={segment == undefined ? 'active' : ''}  href=".">Home</a>
		<a aria-current='{segment === "skill" ? "page" : undefined}' class={segment == 'skill' ? 'active' : ''} href="skill">Skill</a>
	</nav>
	<ul>	
		<li></li>
	</ul>
</div>

