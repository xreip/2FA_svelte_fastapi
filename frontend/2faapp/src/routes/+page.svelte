<script>
	import AccountIcon from '~icons/material-symbols/account-box';
	import PasswordIcon from '~icons/material-symbols/password-rounded';
</script>

<svelte:head>
	<title>Home - Login</title>
	<meta name="Login" content="Login screen" />
</svelte:head>

<section class="flex-[0.8] flex flex-col justify-center items-center">
	<div
		class="flex flex-col border border-p_gray_400 rounded-xl min-h-[30rem] min-w-[30rem] shadow-lg bg-p_gray_150"
	>
		<div class=" p-4 rounded-xl rounded-b-none bg-gradient-to-br from-primary to-primary_b">
			<h1 class="font-bold text-3xl text-center">SIGN IN</h1>
			<h2 class="font-semibold text-xl text-center">to access the portal</h2>
		</div>
		<div class="flex flex-col flex-1 p-12 mt-6 mb-10 ">
			<form action="" class="flex-1 flex flex-col h-full justify-between">
				<div class="flex items-center gap-4 group">
					<AccountIcon height="35" width="35" class="text-primary_b group-hover:text-secondary" />
					<input
						type="email"
						placeholder="Username"
						class="bg-transparent border-b-2 border-b-primary_b p-1 focus:border-b-secondary focus:outline-none focus:border-b-2 flex-1"
					/>
				</div>
				<div class="flex flex-row-reverse items-center gap-4 group">
					<div class="flex-1 z-0">
						<input
							type="password"
							placeholder=" "
							class="bg-transparent border-b-2 border-b-primary_b p-1 focus:border-b-secondary focus:outline-none focus:border-b-2 flex-1 peer block peer"
						/>
						<label
							for="password"
							class="absolute transform -translate-y-6 -z-10 peer-focus:-translate-y-14 peer-focus:scale-75"
							>Password</label
						>
					</div>
					<PasswordIcon
						height="35"
						width="35"
						class="text-primary_b group-hover:text-secondary peer-focus:text-red-300"
					/>
				</div>
				<button
					class="rounded-full text-xl font-bold 
                    bg-gradient-to-br from-primary to-secondary 
                    py-3 px-2 
                    transition-all duration-75 
                    bg-[size:200%] hover:bg-[size:100%] hover:shadow-md hover:shadow-secondary/80
                    hover:outline-2 hover:outline-primary_b hover:outline hover:outline-offset-2
                    active:translate-y-1 active:scale-[97%] active:from-primary/80 active:to-secondary/80
                    active:bg-black">Login</button
				>
			</form>
		</div>
	</div>
</section>
