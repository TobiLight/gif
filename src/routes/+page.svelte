<script lang="ts">
	import { onMount } from 'svelte';
	import imfHero from '../../public/images/imfc.webp';
	import FinancialFreedom from '../../static/financialfreedom.svg';
	import Meter from '$lib/components/icons/Meter.svelte';

	const images = [imfHero, FinancialFreedom];

	let currentImage = 0;
	let currImg = '';

	const showImage = () => {
		currImg = images[currentImage];
		if (currentImage + 1 >= images.length) currentImage = 0;
		else currentImage++;
	};

	onMount(() => {
		const interv = setTimeout(() => {
			showImage();
		}, 500);
		return () => clearInterval(interv);
	});
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
			class="bg-[url('/imfc.webp')] bg-ceter md:bg-top bg-cover bg-no-repeat h-auto w-full aspect-video relative home bg-[100%_50%] flex"
		>
			<div
				class="bg-[#0000006c] absolute top-0 left-0 z-[4] w-full h-full p-8 flex justify-center items-center"
			>
				<div class="text-white text-center flex flex-col gap-4 items-center md:w-4/5">
					<h1 class="text-[calc(73*(100vw_/_1170))] md:text-5xl font-bold">
						GLOBAL INNOVATION FUND
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
				<p>Federal Government with IMF Launches GIF, CFDA, and GOVERNMENT GRANTS</p>
			</div>
			<div class="grid md:grid-cols-2 items-stretch">
				<div>
					<div
						class="bg-[url('/h1img.jpg')] bg-top bg-cover h-[150p] py-36 md:py-16 px-12 flex flex-col justify-center"
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
			</div>
		</div>
	</div>
</section>

<section id="about" class="overflow-hidden">
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
					Local livelihoods are not just about income, but rather economic independence—a form of
					resistance to boom-and-bust development and the dehumanization of indigenous communities
					and cultures. We partner with farmers, fisher folk, beekeepers, and artisans and invest in
					diverse local economies that are committed to restoring the environment, establishing a
					fair wage, and showing great resilience in the face of hardship and disaster.
				</p>
				<p>
					A grant is an award of financial assistance in the form of money which is been issued by
					the government to help increase the growth of the economy and the citizen. Anyone can
					apply as long as they are citizens and you have never applied for any type of grant
					before.
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
			<div class="bg-gray-100 p-14 text-3xl font-bold md:grid md:items-center">
				<h2 class="text-center">
					Federal Government with IMF Launches GIF, CFDA, and GOVERNMENT GRANTS, It's a regional
					program serving the whole worldwide
				</h2>
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

<section id="winners-list">
	<h1 class="font-bold text-4xl text-center my-12">GIF WINNERS LIST 2024</h1>
</section>

<section id="services" class="">
	<div class="flex flex-col lg:flex-row w-full">
		<div class="grid w-full bg-black text-white p-8">
			<div class="grid gap-16 p-12">
				<h1 class="text-8xl font-semibold">Services</h1>
				<div class="grid gap-4">
					<p>
						Global Innovation Fund with IMF Launches GOVERNMENT GRANTS , It's Regional Program
						Serving whole worldwide. Local livelihoods are not just about income, but rather
						economic independence. A form of resistance to boom-and-bust development and the
						dehumanization of indigenous communities and cultures. We partner with and support
						financial aid to senior citizens, semi-retired retired, veterans, citizens with
						disabilities, farmers, fisher folk, beekeepers, and artisans and invest in diverse local
						economies that are committed to restoring the environment, establishing a fair wage, and
						showing great resilience in the face of hardship and disaster.
					</p>
					<p>
						A grant is an award of financial assistance in the form of money which is being issued
						by the government to help increase the growth of the economy and the citizen. Anyone can
						apply as long as you are a senior citizen and you have never applied for any type of
						grant before. *Global Innovation Fund finds and funds innovators, transform the lives of
						people living sub-standard living. *GIF and the Global Innovation Fund logo are
						registered trademarks of Global Innovation Fund. Global Innovation Fund is a registered
						charity (number 1171353) company. *GIF takes a zero-tolerance approach to bribery and
						corruption in our activities or in any program or projects that we support.
					</p>
				</div>
			</div>
		</div>
		<div class="p-4 bg-red-500 w-full"></div>
	</div>
</section>

<section id="contact" class="p-6 overflow-hidden w-full">
	<h1 class="font-bold text-4xl text-center my-12">CONTACT</h1>

	<div class="grid gap-8 lg:gap-0 lg:flex">
		<div class="flex flex-col justify-center items-center text-center gap-4">
			<ul class="list-none text-sm">
				<li>United States</li>
				<li>1201 Connecticut Ave NW Suite 600 Washington, DC 20036</li>
			</ul>

			<ul class="text-sm mb-10 grid gap-5">
				<li>+1-6464447323 - Senior Claims Agent</li>
				<li>+1-6464447323 - Senior Claims Agent</li>
				<li>6464447323 - Senior Claims Agent</li>
				<li>globalinnovationfund.claims.agent@financier.com</li>
				<li>Sunday 10:00AM - 3:00PM</li>
				<li>Monday 8:00AM - 6:00PM</li>
				<li>Tuesday 8:00AM - 6:00PM</li>
				<li>Wednesday 8:00AM - 6:00PM</li>
				<li>Thursday 8:00AM - 6:00PM</li>
				<li>Friday 8:00AM - 6:00PM</li>
				<li>Saturday 8:00AM - 6:00PM</li>
			</ul>

			<div class="w-1/2 mx-auto">
				<p>
					*Global Innovation Fund finds and funds innovators, transform the lives of people living
					sub-standard living.
				</p>
				<p>
					*GIF and the Global Innovation Fund logo are registered trademarks of Global Innovation
					Fund. Global Innovation Fund is a registered charity (number 1171353) company.
				</p>
				<p>*GIF takes a zero-toler</p>
			</div>
		</div>
		<div class="form w-full">
			<form action="#" method="POST" class="w-full grid gap-6">
				<div class="flex items-center gap-6 w-full">
					<label for="name" class="w-full">
						<input type="text" placeholder="Name" class="bg-gray-200 rounded p-4 w-full" />
					</label>
					<label for="phone" class="w-full">
						<input type="phone" placeholder="Phone" class="bg-gray-200 rounded p-4 w-full" />
					</label>
				</div>
				<label for="email">
					<input type="email" placeholder="Email address" class="bg-gray-200 rounded p-4 w-full" />
				</label>
				<label for="message">
					<textarea placeholder="Message" class="bg-gray-200 rounded p-4 w-full" rows="4" cols="6"
					></textarea>
				</label>
				<button class="bg-black p-4 rounded text-white text-lg">Send message</button>
			</form>
		</div>
	</div>
</section>
