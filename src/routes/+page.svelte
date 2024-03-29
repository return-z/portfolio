<script>
	let src = '../lib/profile_pic.jpeg';
	function handleOpen() {
		const desc = document.getElementById('description');
		desc.hidden = !desc.hidden;
	}
</script>

<body class="h-screen w-screen">
	<div id="app" class="flex flex-row">
		<div
			id="left-part"
			class="flex grow text-white w-1/5 h-screen bg-violet-500 justify-center items-center"
		>
			<div id="info" class="flex flex-col">
				<p class="p-2 text-2xl">Vinayak Tyagi</p>
				<p class="p-2 text-2xl">GitHub</p>
				<p class="p-2 text-2xl">LinkedIn</p>
				<p class="p-2 text-2xl">Instagram</p>
			</div>
		</div>
		<div id="right-part" class="flex grow h-screen justify-center w-4/5">
			<div class="w-full">
				<h1 class="text-2xl p-4 text-center">Welcome to my portfolio</h1>

				<div id="education" class="p-4">
					<div class="border border-black p-4">
						<div class="flex justify-between">
							<p>Education</p>
							<button on:click={handleOpen}>Open</button>
						</div>
						<p id="description">Completed formal education from xxx</p>
					</div>
				</div>

				<div id="work-ex" class="p-4">
					<div class="border border-black p-4">
						<p>Work Experience</p>
						<p>Uber</p>
						<p>VComply</p>
					</div>
				</div>

				<div id="projects" class="p-4">
					<div class="border border-black p-4">
						<p>Projects</p>
						<p>Go</p>
						<p>JSEditor</p>
					</div>
				</div>
			</div>
		</div>
	</div>
</body>
