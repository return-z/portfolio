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
			class="flex grow fixed hidden md:flex w-1/5 text-white h-full bg-gradient-to-r from-purple-400 to-pink-600 justify-center items-center"
		>
			<Socials />
		</div>
		<div id="right-part" class="flex md:pl-[20%] grow h-screen justify-center">
			<div class="w-full">
				<h1 class="text-7xl p-4 text-center font-thin">My Portfolio</h1>
				<Education />
				<WorkEx />
				<Projects />
			</div>
		</div>
	</div>
</body>
