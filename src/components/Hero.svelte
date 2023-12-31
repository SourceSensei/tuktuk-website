<script>
	import { onMount } from 'svelte';
	import video from '../public/video/hero-video.mp4';

	let showContent = false;

	onMount(() => {
		// Definindo showContent como verdadeiro para mostrar a div após o montagem do componente
		showContent = true;
	});
</script>

<div>
	<section class="w-full h-auto relative">
		<div class="flex h-screen justify-center items-center flex-col">
			<video class="w-full h-screen object-cover" autoplay loop muted>
				<source src={video} type="video/mp4" />
			</video>

			{#if showContent}
				<div class="w-full h-full flex flex-col justify-center items-center backdrop-brightness-50">
					<div>
						<span class="text-white text-4xl w-1/2 text-center"> Ready for your next tour? </span>
					</div>
					<div class="mt-10">
						<button class="button">Lets go!</button>
					</div>
				</div>
			{/if}
		</div>
	</section>
</div>

<style>
	video {
		/* Adicione estilos para o vídeo conforme necessário */
		object-fit: cover;
		position: absolute;
		top: 0;
		left: 0;
		z-index: -1;
	}

	.button {
		position: relative;
		width: 130px;
		height: 50px;
		background-color: #020202;
		display: flex;
		align-items: center;
		color: white;
		flex-direction: column;
		justify-content: center;
		border: none;
		padding: 12px;
		gap: 12px;
		border-radius: 8px;
		cursor: pointer;
	}

	.button::before {
		content: '';
		position: absolute;
		inset: 0;
		left: -4px;
		top: -1px;
		margin: auto;
		width: 138px;
		height: 58px;
		border-radius: 10px;
		background: linear-gradient(-45deg, #e81cff 0%, #40c9ff 100%);
		z-index: -10;
		pointer-events: none;
		transition: all 0.6s cubic-bezier(0.175, 0.885, 0.32, 1.275);
	}

	.button::after {
		content: '';
		z-index: -1;
		position: absolute;
		inset: 0;
		background: linear-gradient(-45deg, #fc00ff 0%, #00dbde 100%);
		transform: translate3d(0, 0, 0) scale(0.95);
		filter: blur(20px);
	}

	.button:hover::after {
		filter: blur(30px);
	}

	.button:hover::before {
		transform: rotate(-180deg);
	}

	.button:active::before {
		scale: 0.7;
	}
</style>
