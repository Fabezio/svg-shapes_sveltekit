<script>
	const y1 = 10;
	const x1 = 10;
	const length = 50;
	const base = 10;
	const line = base + length;
	const sw = 1;
	const number = 3;
	const stroke = 'black';
	// const x=10
	// const x1=10
</script>

<svg
	version="1.1"
	baseProfile="full"
	width={2 * base + length}
	height={2 * length}
	xmlns="http://www.w3.org/2000/svg"
>
	<line id="left" x1={base} x2={base} y1={base} y2={line} {stroke} stroke-width={sw} />
	<line id="bottom" x1={base} x2={line} y1={line} y2={line} {stroke} stroke-width={sw} />
	<line id="right" x1={line} x2={line} y1={base} y2={line} {stroke} stroke-width={sw} />

	<!-- 

    <rect width="100%" height="100%" fill="red" />

  <circle cx="150" cy="100" r="80" fill="green" />

  <text x="150" y="125" font-size={line} text-anchor="middle" fill="white">SVG</text> -->
</svg>

<style>
	.hidden {
		display: hidden;
	}
</style>
