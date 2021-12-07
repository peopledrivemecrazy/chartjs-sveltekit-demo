<script>
	import Chart from 'chart.js/auto';

	function chart(ctx) {
		const myChart = new Chart(ctx, {
			type: 'bar',
			data: {
				labels: ['Red', 'Blue', 'Yellow', 'Green', 'Purple', 'Orange'],
				datasets: [
					{
						label: '# of Votes',
						data: [12, 19, 3, 5, 2, 3],
					}
				]
			}
		});
	}
</script>

<div>
	<canvas use:chart />
</div>

<style>
	div {
		width: 400px;
		height: 400px;
	}
</style>
