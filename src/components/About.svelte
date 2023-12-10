<div class="w-full relative px-6">
	<section class="container mx-auto">
		<div class="flex flex-col lg:flex-row justify-between">
			<div class="w-full lg:w-1/2 py-12 md:py-20 pr-6 md:pr-24 relative z-10">
				<h2 class="text-2xl md:text-4xl font-extrabold leading-tight text-white">
					About
					<span class="relative"
						><span class="z-10 text-black relative">me</span><span
							class="absolute w-full h-4 bg-indigo-300 left-0 bottom-0"
						></span></span
					>
				</h2>
				<p class="pt-8 text-white text-lg mx-auto">
					Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec lacinia metus ut velit
					congue, nec imperdiet arcu sollicitudin.
				</p>
				<div class="pt-8">
					<button class="button"> Find Out More </button>
				</div>
			</div>
			<!-- <div class="flex flex-col bg-white border shadow-sm rounded-xl dark:bg-slate-900 dark:border-gray-700 dark:shadow-slate-700/[.7]">
				<img class="w-full h-[400px] rounded-t-xl" src="https://images.unsplash.com/photo-1680868543815-b8666dba60f7?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=2532&q=80" alt="Image Description">
				<div class="p-4 md:p-5">
				  <h3 class="text-lg font-bold text-gray-800 dark:text-white">
					Card title
				  </h3>
				  <p class="mt-1 text-gray-500 dark:text-gray-400">
					Some quick example text to build on the card title and make up the bulk of the card's content.
				  </p>
				  <a class="mt-2 py-2 px-3 inline-flex justify-center items-center gap-x-2 text-sm font-semibold rounded-lg border border-transparent bg-blue-600 text-white hover:bg-blue-700 disabled:opacity-50 disabled:pointer-events-none dark:focus:outline-none dark:focus:ring-1 dark:focus:ring-gray-600" href="#">
					Go somewhere
				  </a>
				</div>
			  </div> -->
			  <div class="overflow-hidden rounded-2xl has-shadow w-[30rem] relative">
				<div>
					<img
						src="https://images.unsplash.com/photo-1477959858617-67f85cf4f1df?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1244&q=80"
						class="aspect-video"
						alt=""
					/>
				</div>
				<div class="absolute inset-0 z-10 bg-gradient-to-t from-black" />
				<div class="absolute inset-x-0 bottom-0 z-20 p-4 text-white">
					<div class="text-xs">Ricco Xie • 1 June 2023</div>
					<h3 class="text-xl font-semibold">Sira team talk</h3>
					<div class="text-sm opacity-80">
						<p>
							🕹 Customizable and 😍 accessible design system which provides
							TailwindCSS component class name library to build modern UI. 💥
						</p>
					</div>
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
</style>
