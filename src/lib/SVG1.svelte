<script>
	const length = 50;
	const base = 10;
	const line = base + length;
	const sw = 1;

	const stroke = 'black';
</script>

<svg
	version="1.1"
	baseProfile="full"
	width={2 * base + length}
	height={2 * length}
	xmlns="http://www.w3.org/2000/svg"
>
	<line id="left" x1={base} x2={base} y1={base} y2={line} {stroke} stroke-width={sw} />
</svg>
