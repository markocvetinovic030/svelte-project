<script>
	let img = '../src/img/hero.png';
</script>

<div class="bg-gray-50">
	<div id="container" class="w-8/12 m-auto flex  pt-20 pb-20">
		<div class="w-1/2">
			<h1 class="text-6xl font-bold text-orange-500 pt-20 mb-20 m-auto ">Send Message to Us</h1>
			<p class="text-lg text-orange-500">
				Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas nec est velit. Vestibulum
				non tellus laoreet, vehicula nibh ut, dictum metus. Proin urna justo, feugiat eget turpis
				condimentum, rutrum ornare neque.
			</p>
			<br />

			<p class="text-lg text-orange-500">
				Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas nec est velit. Vestibulum
				non tellus laoreet, vehicula nibh ut, dictum metus.
			</p>
			<br />
			<p class="text-lg text-orange-500">
				Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas nec est velit. Vestibulum
				non tellus laoreet, vehicula nibh ut, dictum metus. Proin urna justo, feugiat eget turpis
				condimentum, rutrum ornare neque.
			</p>
			<br />
			<p
				class="  inline-block font-bold text-xl text-orange-400 hover:text-orange-600  transition-all duration-300 pb-2 cursor-pointer "
			>
				More info...
			</p>
		</div>
		<div class="w-1/2">
			<form class="text-center p-20">
				<label class=" text-orange-400 font-bold text-lg" for="name">Name:</label><br />
				<input
					class="bg-orange-200 mt-4 mb-10 w-72 h-8 hover:bg-orange-300 transition-all duration-300 text-white p-6 outline-none rounded-3xl"
					type="text"
					id="name"
					name="name"
				/><br />
				<label class=" text-orange-400 font-bold text-lg" for="password">Email:</label><br />
				<input
					class="bg-orange-200 mt-4 mb-10 w-72 h-8 hover:bg-orange-300 transition-all duration-300 text-white p-6 outline-none rounded-3xl"
					type="text"
					id="email"
					name="email"
				/><br />

				<label class=" text-orange-400 font-bold text-lg" for="comment">Message:</label><br />
				<textarea
					class=" ml- bg-orange-200 mt-4 mb-10 w-72 hover:bg-orange-300 transition-all duration-300 text-white p-6 outline-none rounded-3xl"
					name="comment"
					form="usrform"
				/>
				<input
					class=" block m-auto text-white font-bold bg-orange-400 p-2 mt-4 w-40 rounded-3xl hover:bg-orange-600 transition-all duration-300"
					type="submit"
					id="submit"
					name="submit"
				/>
			</form>
		</div>
	</div>
	<img class=" m-auto pb-40" src={img} alt="hero" />
</div>
