<script>
	import '$styles/tailwind.css';
	import '$styles/global.css';
	import '$styles/tabs.css';
	import Footer from '$lib/Footer.svelte';
</script>

<svelte:head>
	<title>CORE Vault</title>
</svelte:head>

<main>
	<section>
		<h1>Next Generation Smart Contract Governance</h1>
		<p>
			coreDAO is a fully decentralized autonomous organization which is using a combination of
			governance systems to achieve its on-chain governance and execution.
		</p>
	</section>
	<slot />
</main>
<Footer />

<style lang="postcss">
	* {
		@apply text-white;
	}
	section {
		@apply m-auto text-center;
		max-width: 90ch;
	}
	p {
		@apply text-xl opacity-80;
	}
	main {
		@apply flex overflow-auto text-center font-win  md:mt-20 md:block h-[var(--h-without-footer)] w-[100%] justify-center items-center flex-col;
	}
	h1 {
		@apply text-3xl;
	}
</style>
