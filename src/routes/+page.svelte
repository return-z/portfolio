<script>
	import Socials from './Socials.svelte';
	import Education from './Education.svelte';
	import WorkEx from './WorkEx.svelte';
	import Projects from './Projects.svelte';
</script>

<body class="h-screen w-screen overflow-auto">
	<div id="app" class="flex flex-row grow">
		<div
			id="left-part"
			class="flex fixed grow text-white w-1/5 h-full bg-gradient-to-r from-purple-400 to-pink-600 justify-center items-center"
		>
			<Socials />
		</div>
		<div id="right-part" class="flex ml-[20%] grow h-screen justify-center">
			<div class="w-full">
				<h1 class="text-4xl p-4 text-center font-bold">Welcome to my portfolio</h1>
				<Education />
				<WorkEx />
				<Projects />
			</div>
		</div>
	</div>
</body>
