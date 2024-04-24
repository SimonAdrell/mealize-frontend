<script>
	export let name = 'Day';
	export let food = '';
	function onMouseOver() {
		console.log('mouseover');
	}
</script>

<div class="row" on:focus={onMouseOver}>
	<div class="info">
		<b> {name}</b>
		<span> {food}</span>
	</div>
	<div class="action">
		<div>
			<svg
				width="17"
				height="17"
				viewBox="0 0 24 24"
				fill="none"
				xmlns="http://www.w3.org/2000/svg"
			>
				<path
					d="M4 12.6111L8.92308 17.5L20 6.5"
					stroke="#000000"
					stroke-width="2"
					stroke-linecap="round"
					stroke-linejoin="round"
				/>
			</svg>
		</div>
		<div>
			<svg
				width="17"
				height="17"
				viewBox="0 0 24 24"
				fill="none"
				xmlns="http://www.w3.org/2000/svg"
			>
				<path
					d="M15.4998 5.49994L18.3282 8.32837M3 20.9997L3.04745 20.6675C3.21536 19.4922 3.29932 18.9045 3.49029 18.3558C3.65975 17.8689 3.89124 17.4059 4.17906 16.9783C4.50341 16.4963 4.92319 16.0765 5.76274 15.237L17.4107 3.58896C18.1918 2.80791 19.4581 2.80791 20.2392 3.58896C21.0202 4.37001 21.0202 5.63634 20.2392 6.41739L8.37744 18.2791C7.61579 19.0408 7.23497 19.4216 6.8012 19.7244C6.41618 19.9932 6.00093 20.2159 5.56398 20.3879C5.07171 20.5817 4.54375 20.6882 3.48793 20.9012L3 20.9997Z"
					stroke="orange"
					stroke-width="2"
					stroke-linecap="round"
					stroke-linejoin="round"
				/>
			</svg>
		</div>
		<div>
			<svg
				width="17"
				height="17"
				viewBox="0 0 17 19"
				fill="green"
				xmlns="http://www.w3.org/2000/svg"
			>
				<path
					fill-rule="evenodd"
					clip-rule="evenodd"
					d="M13.9725 14.5664C13.1677 15.7864 11.9729 16.6961 10.5856 17.1452C5.47864 18.791 1.94813 14.892 1.63045 10.8456L4.41729 10.8786C4.67627 13.2755 6.78253 15.5306 9.79238 14.5593C10.9125 14.1984 11.8351 13.6895 12.3696 12.9535L8.48004 13.1847L8.35367 10.4081L15.8611 10.9402L16.4301 18.3488L13.6765 18.4926L13.9725 14.5664ZM6.84048 5.07223C5.83897 5.39626 4.9927 5.83494 4.44168 6.45084L8.32585 6.22264L8.45222 8.99928L0.94474 8.46711L0.375779 1.05853L3.12935 0.914733L2.83435 4.82795C3.62991 3.7235 4.7573 2.9032 6.05032 2.48797C11.0195 0.886518 14.4973 4.53524 14.9728 8.46109L12.2249 8.79435C11.9851 6.38616 9.87249 4.09508 6.84048 5.07223Z"
					fill="green"
				/>
			</svg>
		</div>
	</div>
</div>

<style>
	.row {
		display: grid;
		align-items: center;
		grid-template-columns: 4fr 2fr;
		gap: 1em;
		padding: 1em;
		margin: 1em;
		background: #ecebeb;
		border-radius: 0.2em;
	}
	.row:hover {
		background: #a65757;
	}
	.info {
		display: grid;
		align-items: end;
		grid-template-rows: 1fr;
		font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
	}
	.day {
		font-size: 1.2em;
	}
	.action {
		display: grid;
		align-items: end;
		grid-template-columns: 1fr 1fr 1fr;
		margin: 0.4em;
	}
	.action:hover {
		color: black;
	}

	.action > div > svg:hover {
		height: 20;
		width: 20;
		fill: aquamarine;
	}
</style>
