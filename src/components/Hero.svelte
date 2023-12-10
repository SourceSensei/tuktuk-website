<div class="w-full px-6 py-6 md:py-20">
	<section class="container mx-auto h-90vh">
		<div class="h-full flex flex-col">
			<div class="max-w-xl lg:max-w-3xl mx-auto text-center">
				<h1 class="font-extrabold text-4xl lg:text-5xl leading-tight text-white">
					Ready for a quick
					<span
						class="text-gradient bg-gradient-to-r from-purple-800 to-blue-900 bg-clip-text text-transparent"
					>
						tour?
					</span>
				</h1>
				<div class="pt-10">
					<div class="rounded overflow-hidden shadow-xl relative flex justify-center items-center">
						<button
							aria-label="Play video"
							class="z-10 absolute rounded-full w-24 h-24 bg-indigo-500 flex justify-center items-center hover:bg-indigo-600 transition-colors duration-200 outline-none focus:shadow-outline hover:shadow-outline"
						>
							<svg
								xmlns="http://www.w3.org/2000/svg"
								width="24"
								height="24"
								viewBox="0 0 24 24"
								fill="none"
								stroke="currentColor"
								stroke-width="2"
								stroke-linecap="round"
								stroke-linejoin="round"
								class="text-white"
							>
								<polygon points="5 3 19 12 5 21 5 3"></polygon>
							</svg>
						</button>
						<div
							class="bg-black absolute inset-0 transition-colors duration-200 bg-opacity-25"
						></div>
						<video muted="" playsinline="" class="w-full">
							<source src="" type="video/mp4" class="" />
						</video>
					</div>
				</div>
				<!-- <p class="pt-12 text-gray-600 text-xl">
					Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean nec ex sed nulla gravida
					viverra vitae vel libero.
				</p> -->
				<div class="pt-8 md:pt-10 inline-grid grid-flow-row md:grid-flow-col gap-4">
					<button class="button"> Find Out More </button>
				</div>
			</div>
		</div>
	</section>
</div>

<style>
	.button {
		position: relative;
		width: 130px;
		height: 50px;
		background-color: #000;
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

	.h-90vh {
		height: 90vh;
	}
</style>
