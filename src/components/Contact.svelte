<div class="w-full py-12 md:py-20 px-6">
	<section class="container mx-auto">
		<div class="grid grid-flow-row lg:grid-cols-2 gap-10 md:gap-12">
			<div class="col-span-1">
				<h2 class="text-2xl md:text-6xl font-extrabold leading-none text-white">
					Contact now<br />to book
					<span class="relative"
						><span class="z-10 relative text-white">your tour</span><span
							class="absolute w-full h-6 left-0 bottom-0"
						></span></span
					>
				</h2>
			</div>
			<div class="col-span-1">
				<div class="grid grid-flow-row sm:grid-cols-2 gap-4">
					<div class="flex flex-col">
						<label class="font-bold" for="contact1-name">Name</label><input
							type="text"
							id="contact1-name"
							placeholder="Your Name"
							class="flex-1 mt-1 py-4 transition-all duration-200 rounded border h-12 px-4 border-gray-400 focus:shadow-outline focus:border-blue-500 outline-none w-full"
						/>
					</div>
					<div class="flex flex-col">
						<label class="font-bold" for="contact1-email">Email</label><input
							type="email"
							id="contact1-email"
							placeholder="Your Email"
							class="flex-1 mt-1 py-4 transition-all duration-200 rounded border h-12 px-4 border-gray-400 focus:shadow-outline focus:border-blue-500 outline-none w-full"
						/>
					</div>
				</div>
				<div class="pt-4 flex flex-col">
					<label class="font-bold" for="contact1-message">Message</label><textarea
						id="contact1-message"
						placeholder="Your Message"
						rows="7"
						class="flex-1 mt-1 py-4 transition-all duration-200 rounded border h-12 px-4 border-gray-400 focus:shadow-outline focus:border-blue-500 outline-none w-full"
					></textarea>
				</div>
				<div class="pt-6">
					<button class="button"> Send </button>
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
