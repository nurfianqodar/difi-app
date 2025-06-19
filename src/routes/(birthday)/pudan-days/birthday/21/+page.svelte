<script lang="ts">
	import quotes from '$lib/quotes';
	import IconLoveLetter from '../../../../../components/icons/IconLoveLetter.svelte';
	import ParticleCake from '../../../../../components/particles/ParticleCake.svelte';
	import ParticlePartyPopper from '../../../../../components/particles/ParticlePartyPopper.svelte';
	import ParticleStar from '../../../../../components/particles/ParticleStar.svelte';
	import Main from '../../../../../components/ui/Main.svelte';
	import Section from '../../../../../components/ui/Section.svelte';

	var quote = $state(quotes[Math.floor(Math.random() * quotes.length)]);

	var shuffleQuote = () => {
		quote = quotes[Math.floor(Math.random() * quotes.length)];
	};
</script>

<!-- Start Component -->
<Main>
	<Section>
		<div class="relative flex h-screen flex-col justify-center py-20">
			<ParticleCake className="w-16 h-16 top-5 rotate-12" />
			<ParticleCake className="w-10 h-10 top-10 right-10 -rotate-6" />
			<ParticleStar className="w-24 h-24" />
			<ParticlePartyPopper className="bottom-5 right-16 w-14 h-14" />
			<h1
				class="bg-gradient-to-br from-purple-400 via-pink-300 to-purple-700 bg-clip-text text-center text-6xl font-bold text-transparent"
			>
				Happy Birthday Pudan!! <span class="text-5xl text-black">🥳</span>
			</h1>

			<p class="font-dancing my-5 text-center text-3xl leading-relaxed font-medium text-purple-700">
				{'May this special day bring you boundless happiness,'}
				<br />
				{'everlasting health, and dreams come true! ✨'}
			</p>
		</div>
	</Section>

	<Section>
		<div class="container flex items-center justify-center">
			<div class="relative max-w-xl bg-purple-50 px-5 py-10 leading-relaxed shadow-lg">
				<IconLoveLetter className="absolute fill-pink-500 -top-5 opacity-75" />
				<h2 class="text-center text-3xl text-purple-800">
					For My Beloved <div class="text-5xl font-semibold">Diva Tari Asina Munthe</div>
				</h2>
				<div class="font-dancing mt-10 flex flex-col gap-y-3 text-xl">
					<p>
						Untuk boru ni raja,
						<br />
						Selamat bertambah dewasa
						<br />
						Kamu tidak bisa kembali sedetikpun untuk tidak menyesali masa lalu
						<br />
						Dan kamu tidak pernah tahu rencana tuhan untuk hari esokmu
						<br />
						Tapi hingga detik ini tuhan memberi dinamika kehidupan yang membuatmu belajar bagaimana bersiap
						dengan pelbagai misteri
						<br />
						Bersyukurlah dengan segala rintangan dan nikmatnya
					</p>
					<p>
						Untuk wanita hebat,
						<br />
						Berbangga dirilah dengan segala yang membuat sang pengagum takjub
						<br />
						Angkuhlah dengan semua emas permata yang kamu miliki
						<br />
						Emas permata yang ditambang dengan hati dan ditempa dengan rasa sakit
						<br />
						Percayalah pada semua kekayaan hati yang dapat membeli kasih-Nya
					</p>
					<p>
						Untuk wanitaku,
						<br />
						Maafkan sang pengagum dengan segala kekhilafannya
						<br />
						Maafkan sang pengagum dengan segala ketidaksempurnaannya
						<br />
						Sang pengagum hanya bisa mempersembahkan munajat dan semua yang dimilikinya
						<br />
						Dan terima kasih untukmu yang tak pernah berpaling pada semua kilauan
					</p>
					<div>
						<i class="text-xs">~ Nurfian Qodar</i>
						<p>Selamat ulang tahun ya pudan :)</p>
					</div>
				</div>
			</div>
		</div>
	</Section>
	<Section>
		<div class="my-20">
			<h2 class="text-center text-4xl text-purple-800">Your Reminder</h2>
			<div class="container bg-purple-100">
				<div class="m-5 h-48 bg-white p-3 text-center text-xl">{quote.quote}</div>
				<button onclick={shuffleQuote} class="m-3 rounded-lg bg-purple-800 px-3 py-2 text-white"
					>Shuffle</button
				>
			</div>
		</div>
	</Section>
	<Section>
		<div class="my-5 flex items-center justify-center">
			<a href="/pudan-days/birthday/21/easter-egg">Easter Egg</a>
		</div>
	</Section>
</Main>
<!-- End Component -->
