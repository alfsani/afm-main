<script>
	import Social from '../atoms/Social.svelte';

	// import dua ikon dari iconoir
	import { TwitterIcon } from '@indaco/svelte-iconoir/twitter';
	import { TelegramIcon } from '@indaco/svelte-iconoir/telegram';
</script>

<div class="socials-container">
	<!-- Twitter -->
	<Social tip="Twitter" link="https://twitter.com/username_kamu">
		<TwitterIcon color="var(--accent)" size="22px" />
	</Social>

	<!-- Telegram -->
	<Social tip="Telegram" link="https://t.me/username_kamu">
		<TelegramIcon color="var(--accent)" size="22px" />
	</Social>

	<!-- DexScreener -->
	<Social tip="DexScreener" link="https://dexscreener.com/yourtokenlink">
		<img src="/dexscreener.svg" alt="DexScreener" class="icon" />
	</Social>
</div>

<style>
	.socials-container {
		display: flex;
		gap: 0.75rem;
		align-items: center;
	}

	/* Style untuk ikon DexScreener */
	.icon {
	width: 22px;
	height: 22px;
	object-fit: contain;
	vertical-align: middle;
	opacity: 0.6;  /* atur transparansi ikon */
	transition: opacity 0.3s ease, transform 0.2s ease;
}

.icon:hover {
	opacity: 1;    /* jadi solid saat hover */
	transform: scale(1.05);
}



</style>
