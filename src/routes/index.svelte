<script context="module" lang="ts">
	import Hl from '$lib/Highlight.svelte';
	import Dots from '$lib/Dots.svelte';

	export const prerender = true;
	export const hydrate = false;
	export const router = false;
</script>

<svelte:head>
	<title>Академикс | Максим Тумозов</title>
</svelte:head>

<div class="text">
	<h1>Здравствуйте.</h1>
	<p>
		Я Максим Тумозов, — школьник, знаток английского и программист-самоучка. Понемногу занимаюсь
		веб-разработкой уже более двух лет: начинал с <Hl c="#0769ad">jQuery</Hl>, пару раз пробовал
		<Hl c="#61dafb">React</Hl>
		с <Hl c="#0070f3">Next.js</Hl>, а затем влюбился в <Hl c="#ff3e00">Svelte</Hl> и
		<Hl c="#ff3e00">SvelteKit</Hl>. Их и использую.
	</p>
	<h1>Мои проекты.</h1>
	<p>
		Могу отметить лишь веб-сайт для игрового сервера <Hl c="#dc5b7b" href="https://terraria.tk"
			>Terraria Minigames</Hl
		>, поскольку из всего мной сделанного, только он всё ещё работает и публично доступен. Также уже
		более полугода я работаю над собственным крупным проектом, который использует аж 4 разных языка
		программирования: <Hl c="#35709f">Python</Hl>,
		<Hl c="#9b4f97">C#</Hl>, <Hl c="#69d7e4">Go</Hl> и даже <Hl c="#0101dc">Lua</Hl>.
	</p>
	<h1>Мотивация.</h1>
	<p>
		Очень бы хотел попасть на курс разработчика на платформе <Hl
			c="#1ec988"
			href="https://acdmx.ru/">Академикс</Hl
		> с надеждой получить важный опыт работы в команде, которого мне сейчас не хватает, и попрактиковаться
		в своих навыках.
	</p>
	<p>— yours truly, Максим Тумозов.</p>
</div>

<Dots w={25} h={30} x="22vw" y="2vh" color="#113" />
<Dots w={20} h={15} x="52vw" y="58vh" color="#210c30" />

<footer>
	<span>@btvoidx</span>
	<a target="_blank" rel="noopener noreferrer" href="https://vk.com/btvoidx">VK</a>
	<a target="_blank" rel="noopener noreferrer" href="https://github.com/btvoidx">GitHub</a>
	<a target="_blank" rel="noopener noreferrer" href="mailto:maksimtumozov@gmail.com">E-mail</a>
	<a target="_blank" rel="noopener noreferrer" href="https://github.com/btvoidx/acdmx-application"
		>Код сайта</a
	>
</footer>

<style lang="postcss">
	.text {
		@apply px-6 text-gray-100 w-full mx-auto mt-6;
		@apply md:w-[75ch] md:mt-16;
	}

	h1 {
		@apply text-3xl mb-2 font-medium;
	}

	p {
		@apply text-2xl mb-6 leading-7 font-normal tracking-[-0.02em];
	}

	footer {
		@apply px-6 text-gray-300 w-full mx-auto flex gap-x-4 mt-14 mb-6;
		@apply md:w-[75ch];
	}

	footer > a:last-child {
		@apply ml-auto;
	}
</style>
