<script lang="ts">
	import Navbar from '$lib/Navbar.svelte';
	import Box from '$lib/Box.svelte';
	import Show from '$lib/Show.svelte';
</script>

<main class="">
	<div class="main-image">
		<Navbar />
		<div class="">
			<div>
				<p
					class="
                gf text-center text-[#00ED82] pb-[8px]
                 font-[600] tracking-[.6px ] text-[12px]
    
                "
				>
					DISNEY BUNDLE TRIO BASIC
				</p>
			</div>

			<div class="flex justify-center">
				<div class="flex justify-center flex-col pt-2 pb-2">
					<img
						class="
    
                 w-[500px]
                 opacity-[1] min-h-[auto] "
						src="dis.png"
						alt=""
					/>
				</div>
			</div>
			<div>
				<div>
					<p
						class="text-white text-center 
                gf text-[24px] font-[500] mt-[16px]
                "
					>
						Get Hulu, Disney+, and ESPN+, all with ads, for $12.99/month.
					</p>

					<p class="text-white text-center underline pt-5 pb-3 text-[15px] cursor-pointer">
						Terms Apply
					</p>

					<p class="text-white text-center underline text-[20px] cursor-pointer">
						Sign up for Hulu only
					</p>
					<div class="flex justify-center mt-7">
						<button class="gf rounded-md font-[600] text-center bg-[#1CE783] p-3 w-[500px]">
							GET ALL THREE
						</button>
					</div>
				</div>
			</div>
			<Box />
		</div>
	</div>
	<div class="bg-[#0b0c0f] text-white">
		<div class="p-5">
			<p
				class=" gf text-center text-[#00ED82] pb-[8px]
			font-[600] tracking-[.6px ] text-[15px] mb-2"
			>
				INCLUDED IN ALL PLANS
			</p>
			<h1 class="text-center gf font-[600] text-[30px] mb-2">All The TV You Love</h1>
			<p class="text-center">
				Watch full seasons of exclusively streaming series, current-season episodes, hit movies,
				Hulu Originals, kids shows, and more.
			</p>
			<div class="sm:flex sm:justify-center mt-5 mb-[50px]">
				<div class="flex sm:flex-col gap-5 justify-center">
					<div>
						<Show a="Past & Current Seasons" b="Tv Shows" url="bobs-b.jpg" />
					</div>

					<div>
						<Show a="New & Classic" b="Movies" url="face.jpg" />
					</div>

					<div>
						<Show a="Groundbreaking" b="Hulu Orignals" url="face2.jpg" />
					</div>

					<div>
						<Show a="Add-on" b="Premiums" url="face3.jpg" />
					</div>
				</div>
			</div>
			<div>
				<p
					class=" gf text-center text-[#00ED82] pb-[8px]
				font-[600] tracking-[.6px ] text-[12px] "
				>
					Hulu (With Ads) + LIVE TV, NOW WITH DISNEY+ (WITH ADS) AND ESPN+ (WITH ADS)
				</p>
				<h1 class="text-center gf font-[600] text-[30px]">Live TV Makes It Better</h1>
				<div class="flex justify-center">
					<div class="flex flex-col justify-center w-[500px]">
						<p class="text-center gf font-[500] w-[500px] breakwords">
							Make the switch from cable. Get 85+ top channels on Hulu (With Ads) + Live TV with
							your favorite live sports, news, and events - plus the entire Hulu streaming library.
							With Unlimited DVR, store Live TV recordings for up to nine months and fast-forward
							through your DVR content. Access endless entertainment with Disney+ and live sports
							with ESPN+.
						</p>
						<p class="text-center text-gray-400 text-[10px] mt-5">
							Regional restrictions, blackouts and Live TV terms apply. Access content from each
							service separately. Location data required to watch certain content. Unlimited DVR
							recording is not available for on-demand shows.
						</p>
					</div>
				</div>
			</div>
		</div>
	</div>
</main>
