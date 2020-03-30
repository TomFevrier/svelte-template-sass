<script>
	export let name;
</script>

<main>
	<h1>Hello {name}!</h1>
	<h3>
		<span>Svelte template using </span>
		<img
			class="logo-large"
			alt="Sass logo"
			src="https://sass-lang.com/assets/img/styleguide/color-1c4aab2b.png"
		/>
		<img
			class="logo-small"
			alt="Sass logo"
			src="https://sass-lang.com/assets/img/styleguide/seal-color-aef0354c.png"
		/>
	</h3>
	<p>Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn how to build Svelte apps.</p>
</main>

<style lang='scss'>
	@import './global.scss';

	main {
		text-align: center;
		padding: 1em;
		width: 75%;
		margin: 0 auto;

		h1 {
			text-transform: uppercase;
			font-size: 4em;
			font-weight: 400;
		}

		h3 {
			font-size: 1.4rem;
			font-weight: 400;
			color: #c69;
		}

		img {
			margin: 0 auto;
		}

		.logo-large {
			display: inline-block;
			vertical-align: -1.5rem;
			width: 8rem;
		}

		.logo-small {
			display: none;
		}

		@include md {
			width: 100%;

			h3 {
				font-size: 1.2rem;
			}

			.logo-small {
				display: inline-block;
				vertical-align: middle;
				width: 3rem;
				padding: 0.2rem;
			}

			.logo-large {
				display: none;
			}
		}
	}
</style>
