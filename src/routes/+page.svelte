<script lang="ts">
	import Meter from '$lib/components/icons/Meter.svelte';
	import Location from '$lib/components/icons/Location.svelte';
	import Phone from '$lib/components/icons/Phone.svelte';
	import Envelop from '$lib/components/icons/Envelop.svelte';
	import Table from './Table.svelte';

	let isLoading: boolean = false;

	const about = [
		{
			id: 1,
			title: 'National Community Grant',
			content:
				'Since 1993, NCG has been one of the leading organizations in the world supporting grassroots-led efforts to protect the planet and the rights of people. Together with our diverse community of people on the frontlines and our supporters, we’ve impacted the lives of millions of people.'
		},
		{
			id: 2,
			title: 'What is NCG Program?',
			content:
				'National Community Grant is a charitable foundation that makes small grants (typically $100,000 to $5,000,000) to grassroots environmental causes around the world.'
		},
		{
			id: 3,
			title: 'Mission & Vision',
			content: ''
		}
	];

	const currentAbout = { title: about[0].title, content: about[0].content };
</script>

<section id="#">
	<!-- <div
		class={"bg[url('../../static/financialfreedom.svg')] bg-ceter md:bg-top bg-cover bg-no-repeat h-auto md:h-[600px] w-full aspect-video relative home bg-[100%_50%] flex"}
	>
		<img src={currImg} alt="" class="w-full h-auto object-cover home-bg" />
		<div
			class="bg-[#0000006c] absolute top-0 left-0 z-[4] w-full h-full p-8 flex justify-center items-center"
		>
			<div class="text-white text-center flex flex-col gap-4 items-center md:w-2/3 lg:w-2/4">
				<h1 class="text-[calc(73*(100vw_/_1170))] md:text-5xl font-bold">GLOBAL INNOVATION FUND</h1>
				<p class="text-[calc(73*(100vw_/_2040))] sm:text-[calc(43*(100vw_/_1570))] md:text-xl">
					Creative solutions, creative results. We value honesty, transparency, empathy,
					professionalism and innovation
				</p>
			</div>
		</div>
	</div> -->
	<div class="flex flex-col lg:flex-row items-stretch w-full">
		<div
			class="bg-[url('/imfc.webp')] md:bg-top bg-cover bg-no-repeat h-auto w-full aspect-video relative home bg-[100%_50%] flex"
		>
			<div
				class="bg-[#0000006c] absolute top-0 left-0 z-[4] w-full h-full p-8 flex justify-center items-center"
			>
				<div class="text-white text-center flex flex-col gap-4 items-center md:w-4/5">
					<h1 class="text-[calc(73*(100vw_/_1170))] md:text-5xl font-bold">
						NATIONAL COMMUNITY GRANT
					</h1>
					<p class="text-[calc(73*(100vw_/_2040))] sm:text-[calc(43*(100vw_/_1570))] md:text-xl">
						Creative solutions, creative results. We value honesty, transparency, empathy,
						professionalism and innovation
					</p>
				</div>
			</div>
		</div>
		<div class="flex flex-col lg:grid grid-rows-2 w-full">
			<div class="bg-gray-100 p-14 text-4xl md:grid md:items-center">
				<p>
					NCG - Awarding International Monetary funds for the Retired, Semi retired, Old, Disable,
					Deaf, Widow, Divorced and Workers
				</p>
			</div>
			<div class="grid md:grid-cols-2 items-stretch">
				<div>
					<div
						class="bg-[url('/h1img.jpg')] bg-top bg-cover h-[150p] py-36 md:py-16 px-12 flex flex-col justify-center"
					>
						<Meter class="text-6xl text-gray-400" />
						<div class="grid gap-4 mt-6">
							<h1 class="font-semibold text-4xl">International Monetary funds</h1>
							<p class="text-gray-500">NCG Keeps impacting the lives of millions of people.</p>
						</div>
					</div>
				</div>

				<div
					class="bg-blue-500 pt-36 md:pt-16 pb-14 px-4 flex flex-col gap-6 justify-end text-gray-100"
				>
					<h2 class="text-3xl font-semibold">
						​Achieving global environmental justice, rooted in cultural integrity, led by
						communities and grassroots movements.
					</h2>
				</div>
			</div>
		</div>
	</div>
</section>

<section class="overflow-hidden">
	<!-- <div class="flex flex-col lg:flex-row gap-6 lg:gap-14 md:items-center md:justify-between">
		<div class="flex flex-col max-w-[900px] w-full">
			<div class="flex flex-col gap-4 text-center lg:text-left lg:gap-6">
				<p class="tracking-wider text-xl sm:mx-auto w-full md:mx-0">
					Federal Government with IMF Launches GIF, CFDA, and GOVERNMENT GRANTS, It's Regional
					Program Serving whole worldwide. Local livelihoods are not just about income, but rather
					economic independence—a form of resistance to boom-and-bust development and the
					dehumanization of indigenous communities and cultures.
					<br />
					<br />
					We partner with farmers, fisher folk, beekeepers, and artisans and invest in diverse local
					economies that are committed to restoring the environment, establishing a fair wage, and showing
					great resilience in the face of hardship and disaster A grant is an award of financial assistance
					in the form of money which is been issued by the government to help increase the growth of
					the economy and the citizen. Anyone can apply as long as they are citizens and you have never
					applied for any type of grant before.
				</p>
			</div>
		</div>
		<div class="w-full mx-auto md:ml-[-55px] md:mr-[-103px] sm:w-3/5 md:w-full hero-image">
			<img src={FinancialFreedom} alt="GIF Hero" class="w-full h-full object-cover flex-1" />
		</div>
	</div> -->

	<div class="flex flex-col-reverse lg:flex-row-reverse items-stretch w-full">
		<div class="h-auto w-full aspect-video relative text-2xl grid items-center">
			<!-- <img src={'/financialfreedom1.svg'} alt="GIF Hero" class="w-full h-full object-over flex-1" /> -->
			<div class="p-8 flex flex-col gap-4">
				<p>
					Since 1993, National Community Grant has been one of the leading organizations in the
					world supporting grassroots-led efforts to protect the planet and the rights of people.
					Together with our diverse community of people on the frontlines and our supporters, we’ve
					impacted the lives of millions of people.
				</p>
				<p>
					National Community Grant is different from other international organizations in that we
					don’t try to dictate an agenda from afar. Instead, we trust local people to advance
					solutions and strategies that will best fit their needs, providing them the resources to
					make their ideas a reality.
				</p>
			</div>
			<!-- <div
				class="bg-[#0000006c] absolute top-0 left-0 z-[4] w-full h-full p-8 flex justify-center items-center"
			>
				<div class="text-white text-center flex flex-col gap-4 items-center md:w-3/4">
					<h1 class="text-[calc(73*(100vw_/_1170))] md:text-5xl font-bold">
						GLOBAL INNOVATION FUND
					</h1>
					<p class="text-[calc(73*(100vw_/_2040))] sm:text-[calc(43*(100vw_/_1570))] md:text-xl">
						Creative solutions, creative results. We value honesty, transparency, empathy,
						professionalism and innovation
					</p>
				</div>
			</div> -->
		</div>
		<div class="flex flex-col lg:grid grid-row-2 w-full items-stretch">
			<div class="bg-gray-100 p-14 text-3xl font-bold grid md:grid md:items-center gap-6 md:gap-0">
				<h2 class="text-center">
					National Community Grant is a charitable foundation that makes small grants (typically
					$100,000 to $5,000,000) to grassroots environmental causes around the world.
				</h2>
				<div class="mx-auto">
					<a
						href="/about"
						class="px-4 text-white bg-black rounded hover:bg-transparent hover:text-black border border-transparent hover:border-black"
						>Read more</a
					>
				</div>
			</div>
			<!-- <div class="grid md:grid-cols-2 items-stretch">
				<div>
					<div
						class="bg-[url('../../static/h1img.jpg')] bg-top bg-cover h-[150p] py-36 md:py-16 px-12 flex flex-col justify-center"
					>
						<Meter class="text-6xl text-gray-400" />
						<div class="grid gap-4 mt-6">
							<h1 class="font-semibold text-4xl">Simplify your organization</h1>
							<p class="text-gray-500">Mauris tempus nisl vitae magna pulvinar laoreet nillum.</p>
						</div>
					</div>
				</div>

				<div
					class="bg-blue-500 pt-36 md:pt-16 pb-14 px-4 flex flex-col gap-6 justify-end text-gray-100"
				>
					<h2 class="text-4xl font-semibold">"Understanding the buyer & the process of sale."</h2>
					<p>Jullian Mayer, CEO</p>
				</div>
			</div> -->
		</div>
	</div>
</section>

<section id="winners-list" class="pt-10 pb-20 border-t overflow-hidden">
	<h1 class="font-bold text-4xl text-center my-12">GIF WINNERS LIST 2024</h1>
	<div class="w-11/12 lg:w-2/3 mx-auto">
		<Table />
		<div class="mx-auto text-center text-lg font-semibold mt-8">
			<a
				href="/winners-list"
				class="rounded-full px-4 py-2 text-white bg-black hover:bg-transparent hover:text-black border border-transparent hover:border-black"
				>See full list</a
			>
		</div>
	</div>
</section>

<section id="about" class="">
	<div class="flex flex-col lg:flex-row lg:w-10/12 mx-auto p-4 bg-blue-500 rounded-md">
		<div class="grid w-full">
			<div class="lg:hdden flex">
				<div class="bg-green-400 h-1 w-full"></div>
				<div class="bg-red-400 h-1 w-full"></div>
				<div class="bg-yellow-400 h-1 w-full"></div>
			</div>
			<div class="grid w-full bg-black text-white p-8">
				<div class="grid gap-16 md:p-12">
					<div class="bg-gray-900 p-3 rounded">
						<div class="grid md:grid-cols-3 gap-4 text-center font-semibold">
							{#each about as aboutInfo}
								<button
									on:click={(e) => {
										currentAbout.title = aboutInfo.title;
										currentAbout.content = aboutInfo.content;
									}}
									class="bg-green-400 py-4 rounded"
								>
									<h1>{aboutInfo.title}</h1>
								</button>
							{/each}
						</div>
					</div>
					<h1 class="text-5xl text-center md:text-left md:text-5xl font-semibold">
						{currentAbout.title}
					</h1>
					<div class="flex flex-col gap-8">
						{#if currentAbout.title.includes('Mission & Vision')}
							<div class="flex flex-col gap-1">
								<h1 class="text-xl font-bold underline">Mission</h1>
								<p>
									National Community Grant mobilizes resources for communities worldwide to protect
									our shared planet and work toward a more equitable world.
								</p>
							</div>
							<div class="flex flex-col gap-1">
								<h1 class="text-xl font-bold underline">Vision</h1>
								<p>
									​Achieving global environmental justice, rooted in cultural integrity, led by
									communities and grassroots movements.
								</p>
							</div>
						{:else}
							<p>
								{currentAbout.content}
							</p>
						{/if}
					</div>
				</div>
			</div>
			<div class="lg:hdden flex">
				<div class="bg-green-400 h-1 w-full"></div>
				<div class="bg-red-400 h-1 w-full"></div>
				<div class="bg-yellow-400 h-1 w-full"></div>
			</div>
		</div>

		<!-- <div class="hidden lg:block p-4 bg-red-500 w-full"></div> -->
	</div>
</section>

<section id="contact" class="overflow-hidden w-full">
	<h1 class="font-bold text-4xl text-center my-12">CONTACT</h1>

	<div class="grid gap-8 lg:gap-0 lg:flex w-5/6 md:w-3/4 lg:w-1/2 mx-auto">
		<div class="form w-full">
			<form
				on:submit={(e) => {
					e.preventDefault();
					isLoading = true;

					setTimeout(() => {
						isLoading = false;
					}, 3000);
				}}
				action="#"
				method="POST"
				class="w-full grid gap-6"
			>
				<div class="flex flex-col md:flex-row items-center gap-6 w-full">
					<label for="name" class="w-full">
						<span class="text-lg font-semibold">Name</span>
						<input
							type="text"
							placeholder="Name"
							class="bg-gray-200 rounded p-4 w-full focus-within:ring-0 border-none"
						/>
					</label>
					<label for="phone" class="w-full">
						<span class="text-lg font-semibold"> Phone No </span>
						<input
							type="phone"
							placeholder="Phone"
							class="bg-gray-200 rounded p-4 w-full focus-within:ring-0 border-none"
						/>
					</label>
				</div>
				<div class="flex flex-col md:flex-row items-center gap-6 w-full">
					<label for="email" class="w-full">
						<span class="text-lg font-semibold"> Email </span>
						<input
							type="email"
							placeholder="Email address"
							class="bg-gray-200 rounded p-4 w-full focus-within:ring-0 border-none"
						/>
					</label>
					<label for="age">
						<span class="text-lg font-semibold"> Age </span>
						<input
							type="number"
							placeholder="Age"
							class="bg-gray-200 rounded p-4 focus-within:ring-0 border-none"
						/>
					</label>
				</div>

				<label for="drivers-license">
					<span class="text-lg font-semibold"> Driver's License </span>
					<div class="w-full">
						<div
							class="border-4 border-dashed w-full p-10 border-gray-500 text-2xl text-center text-gray-400"
						>
							<p class="text-6xl">+</p>
							<p>Click here to add an image</p>
						</div>
					</div>
				</label>
				<label for="message">
					<span class="text-lg font-semibold"> Message </span>
					<textarea
						placeholder="Message"
						class="bg-gray-200 rounded p-4 w-full focus-within:ring-0 border-none"
						rows="4"
						cols="6"
					></textarea>
				</label>
				<button
					disabled={isLoading}
					class={`${isLoading ? 'opacity-55' : ''} bg-black p-4 rounded text-white text-lg`}
					>{isLoading ? 'Please wait...' : 'Send message'}</button
				>
			</form>
		</div>
	</div>

	<div class="bg-[url('/Africa.jpg')] bg-top bg-no-repeat text-lg text-white relative flex mt-10">
		<div
			class="w-full h-full justify-center grid lg:grid-cols-3 bg-[#0000006c] relative p-8 items-stretch"
		>
			<div class="p-4 text-center">
				<Location class="mx-auto text-4xl" />
				<p>Head Office: 2840 Wilderness Place, Suite A Boulder, CO 80301. USA​</p>
			</div>
			<div class="p-4 text-center">
				<Phone class="mx-auto text-4xl" />
				<p>USA HQ No: +1(223) 228-2889 South Africa No: +27(6o)633-6340</p>
			</div>
			<div class="p-4 text-center">
				<Envelop class="mx-auto text-4xl" />
				<p>nationalcommunitygrant@safrica.com fiona.ncg@safrica.com</p>
			</div>
		</div>
	</div>
</section>
