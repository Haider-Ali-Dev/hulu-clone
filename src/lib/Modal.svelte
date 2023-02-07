<script lang="ts">
	export let showModal: boolean;
	let password = '';
	let email = '';
	let isValid = false;
	let learnMore = false

	function checkEmailAndPassword() {
		console.log('called');
		if (password.length && email.length) {
			isValid = true;
		} else {
			isValid = false;
		}

		console.log(isValid);
	}
</script>

{#if showModal}
	<div
		class="z-[1] fixed left-0 top-0 w-[100%] h-[100%] flex justify-center  overflow-auto p-5 rounded  bg-[rgba(0,0,0,0.4)]"
	>
		<div class="p-3 w-[600px] bg-white h-[600px] self-center">
			<p
				class="gf font-[600] cursor-pointer text-right text-[20px]"
				on:click={() => (showModal = !showModal)}
			>
				X
			</p>
			<div class="mt-2 p-5">
				<h1 class="gf font-[600] text-[24px] leading-[1.24] tracking-[0.6]">Log In</h1>
				<p class="mt-5 font-[400] text-[14px] leading-[21px] text-[#636E85]">
					You will use this email and password to log into your accounts for all your favorite
					services across The Walt Disney Family of Companies, including Disney+, Hulu and ESPN+.
				</p>
				<div class="mt-5 flex justify-center">
					<div class="w-[90%]">
						<div class="mb-3">
							<p class="block text-[12px] gf tracking-[1.25px] font-[500] text-[#636E85] ">EMAIL</p>
						</div>
						<div>
							<input
							bind:value={email}

								on:change={checkEmailAndPassword}
								class="w-[90%] p-3 font-[16px] border-[2px] border-solid rounded-md"
								type="email"
							/>
						</div>
					</div>
				</div>

				<div class="mt-10 flex justify-center">
					<div class="w-[90%]">
						<div class="mb-3">
							<p
								class="block text-[12px] gf tracking-[1.25px] uppercase font-[500] text-[#636E85] "
							>
								Password
							</p>
						</div>
						<div>
							<input
							bind:value={password}
								on:change={checkEmailAndPassword}
								class="w-[90%] p-3 font-[16px] border-[2px] border-solid rounded-md"
								type="password"
							/>
						</div>
					</div>
				</div>
				<div class="mt-5 flex justify-center">
					<div class="w-[90%]">
						<p class="text-blue-400">Forgot your email or password?</p>
					</div>
				</div>
				<div class="mt-5 flex justify-center">
					<div class="w-[90%]">
						{#if !isValid}
							<button disabled class="bg-[#272C35] rounded-md opacity-50 w-[90%] text-white gf font-[500] p-3"
								>LOGIN</button
							>
						{:else}
							<button class="bg-[#272C35] rounded-md  w-[90%] text-white gf font-[500] p-3">LOGIN</button>
						{/if}
					</div>
				</div>
			</div>
		</div>
	</div>
{/if}
