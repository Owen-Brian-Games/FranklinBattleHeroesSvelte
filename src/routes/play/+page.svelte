<script>
	let choice = $state();
	let info = "Fight!";

	let jacket = "sabercat";

	let selection = $state();

	let run = true;
	function play() {
		while (true) {

		}
	}



</script>

<div class="place-items-center flex flex-col text-2xl">
	<div class="flex flex-row">
		<select class="p-3 rounded-lg text-gray-800 border fixed left-5 w-72 h-16 align-middle" bind:value={choice}>
			<option value="franklin">Original Franklin</option>
			<option value="sabercat">Sabercat Franklin</option>
			<option value="olympian">Olympian Franklin</option>
		</select>
		<button on:click={play} class="p-5 w-60 outline rounded-lg text-center bg-blue-500 fixed left-80 h-16">Start</button>
		<h1 class="text-5xl text-bold">{info}</h1>
	</div>
	<div class="flex flex-row">
		<div class="w-1/2 fixed left-5 mt-5 justify-items-center flex flex-col">
			<img src="src/lib/franklin_jacket_{jacket}.png" height="288" width="288" class="fixed mt-6"/>
			<select bind:value={selection} class="p-3 rounded-lg text-gray-800 border fixed w-72 mt-80">
				<option value="1">1: 25 Damage - 25% Failure</option>
				<option value="2">2: 15 Damage - 0% Failure</option>
				<option value="3">Ability: 100 Damage - 3 points req.</option>
			</select>
			<button class="p-5 w-72 outline rounded-lg text-center bg-blue-500 mt-96 fixed">
				Attack!
			</button>
		</div>
		<div class="w-1/2 fixed right-0 m-5 justify-items-center">
			<img src="src/lib/franklin_jacket_enemy.png" height="288" width="288" class="fixed right-5 mt-10"/>
		</div>
	</div>
</div>