<script>
	import Socials from './Socials.svelte';
	import Education from './Education.svelte';
	import WorkEx from './WorkEx.svelte';
	import Projects from './Projects.svelte';
</script>

<svelte:head>
	<title>Vinayak's Portfolio</title>
</svelte:head>
<body class="h-screen w-screen bg-gradient-to-r from-sky-200 to-orange-200 overflow-auto">
	<div id="app" class="flex flex-row grow">
		<div
			id="left-part"
			class="flex grow fixed hidden md:flex w-1/5 text-black h-full border-r border-white text-black justify-center items-center"
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
