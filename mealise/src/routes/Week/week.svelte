<script>
	import Weekday from './weekday.svelte';
	let weekdays = [
		{
			Name: 'Monday',
			food: 'Potatis med biffar och brunsås'
		},
		{
			Name: 'Tuesday',
			food: 'Pasta med stuvad svamp'
		},
		{
			Name: 'Wednesday',
			food: 'Ärtsoppa'
		},
		{
			Name: 'Thursday',
			food: 'Köttfärssås med spagetti'
		},
		{
			Name: 'Friday',
			food: 'Ris med broccoligryta'
		},
		{
			Name: 'Saturday',
			food: 'Potatismos med falukorv'
		},
		{
			Name: 'Sunday',
			food: 'Hamburgare'
		}
	];
</script>

<div>
	{#each weekdays as weekday}
		<Weekday name={weekday.Name} food={weekday.food}></Weekday>
	{/each}
</div>
