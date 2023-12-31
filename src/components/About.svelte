<script>
	import image from '../public/about-image.jpg';
</script>

<div class="w-full mt-10 mb-10">
	<section class="text-white">
		<div
			class="container flex flex-col justify-center p-6 mx-auto sm:py-12 lg:py-24 lg:flex-row lg:justify-between"
		>
			<div
				class="flex flex-col justify-center p-6 text-center rounded-sm lg:max-w-md xl:max-w-lg lg:text-left"
			>
				<div>
					<h1 class="text-5xl font-bold leadi sm:text-6xl">
						About
						<span class="">me</span>
					</h1>
				</div>
				<div>
					<p class="mt-6 mb-8 text-lg sm:mb-12">
						Dictum aliquam porta in condimentum ac integer
						<br class="hidden md:inline lg:hidden" />turpis pulvinar, est scelerisque ligula sem
					</p>
				</div>

				<div class="flex text-center items-center justify-center">
					<a
						rel="noopener noreferrer"
						href="#"
						class="px-8 py-3 text-lg font-semibold rounded button">Discover</a
					>
				</div>
			</div>
			<div
				class="flex items-center justify-center p-6 mt-8 lg:mt-0 h-72 sm:h-80 lg:h-96 xl:h-112 2xl:h-128"
			>
				<img src={image} alt="" class="object-contain h-72 sm:h-80 lg:h-96 xl:h-112 2xl:h-128" />
			</div>
		</div>
	</section>
</div>

<style>
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
