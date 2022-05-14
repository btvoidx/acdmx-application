<script context="module">
	import Colored from '$lib/Colored.svelte';

	export const prerender = true;
</script>

<svelte:head>
	<title>Академикс | Максим Тумозов</title>
</svelte:head>

<div class="text">
	<h1>Здравствуйте.</h1>
	<p>Я Максим Тумозов, — школьник и программист-самоучка с замашкой на веб-разработчика.</p>
	<p>
		Понемногу занимаюсь веб-разработкой уже более двух лет. Начинал с <Colored c="#0769ad"
			>jQuery</Colored
		>, пару раз пробовал <Colored c="#61dafb">React</Colored> с <Colored c="#0070f3"
			>Next.js</Colored
		>, а затем влюбился в <Colored c="#ff3e00">Svelte</Colored> и <Colored c="#ff3e00"
			>SvelteKit</Colored
		>. Их и использую.
	</p>
	<p>
		До моего увлечения веб-разработкой, я увлекался программированием в целом. Началось с
		робототехники, а потом закрутилось: самостоятельно выучил на приемлимом уровне весь следующий
		список языков. В порядке изучения: <Colored c="#35709f">Python</Colored>, <Colored c="#e9d54c"
			>JavaScript</Colored
		>, <Colored c="#9b4f97">C#</Colored>,
		<Colored c="#007acc">TypeScript</Colored>, <Colored c="#69d7e4">Go</Colored>, <Colored
			c="#0101ff">Lua</Colored
		>.
	</p>
	<p>
		Из собственных проектов могу отметить лишь <Colored c="#dc5b7b"
			><a href="https://terraria.tk" target="_blank" rel="noopener noreferrer">terraria.tk</a
			></Colored
		>, поскольку только он всё ещё работает. Прямо сейчас я работаю над большим проектом, который
		использует всё от <Colored c="#009485">FastAPI</Colored> с <Colored c="#35709f">Python</Colored>
		до <Colored c="#9b4f97">C#</Colored> и <Colored c="#0101ff">Lua</Colored>.
	</p>
</div>

<style lang="postcss">
	.text {
		@apply p-6 text-gray-100 w-full mx-auto;
		@apply md:w-[85ch] md:mt-16;
	}

	h1 {
		@apply text-4xl mb-6;
	}

	p {
		@apply text-2xl mb-4 leading-7;
	}
</style>
