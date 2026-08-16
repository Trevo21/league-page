<script>
	import { Awards } from '$lib/components'
	import { waitForAll } from '$lib/utils/helper';
	import LinearProgress from '@smui/linear-progress';

    export let data;
    const {awardsData, teamManagersData} = data;
</script>

<style>
    .awards {
        display: block;
        margin: 30px auto;
		width: 95%;
		max-width: 1000px;
		position: relative;
		z-index: 1;
		overflow-y: hidden;
    }

	.loading {
		display: block;
		width: 85%;
		max-width: 500px;
		margin: 80px auto;
	}

	.nothingYet {
		display: block;
		width: 85%;
		max-width: 500px;
		margin: 80px auto;
		text-align: center;
	}
</style>

<div class="awards">
	{#await waitForAll(awardsData, teamManagersData) }
		<div class="loading">
			<p>Retrieving awards data...</p>
			<LinearProgress indeterminate />
		</div>
	{:then [podiums, leagueTeamManagers] }
		{#each podiums as podium}
			<Awards {podium} {leagueTeamManagers} />
		{:else}
			<p class="nothingYet">No seasons have been completed yet, so no awards have been earned...</p>
		{/each}
	{:catch error}
		<!-- promise was rejected -->
		<p>Something went wrong: {error.message}</p>
	{/await}
</div>
<div class="history">
	<h3>2022 Awards</h3>

	<img src="/banner.png" class="banner" alt="The Phoenix" />

	<div id="podium">
		<img src="/podium.png" class="podiumImage" alt="podium" />

		 champs
		<img src="/managers/james.jpg" class="first champ" alt="champion" />
		<img src="/laurel.png" class="laurel" alt="laurel" />
		<p><span class="label firstLabel"> James </span></p>

		<img src="/managers/james.jpg" class="second champ" alt="2nd" />
		<p><span class="label firstLabel"> James </span></p>
		<img src="/managers/james.jpg" class="third champ" alt="3rd" />
		<p><span class="label thirdLabel"> James </span></p>
	</div>
</div>