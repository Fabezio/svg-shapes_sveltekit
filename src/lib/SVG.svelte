<script>
  const y1=10
  const x1=10
    const length=50
    const base=10
    const line=base+length
    const sw=3
    // const x=10
    // const x1=10
</script>

<svg version="1.1"
     baseProfile="full"
     width={2*length} height={2*length}
     xmlns="http://www.w3.org/2000/svg">
    
     <line id="left" 
     x1={base} 
     x2={base} 
     y1={base} 
     y2={line} 
     stroke="black" 
     stroke-width={sw} />
     <line id="bottom" 
     x1={base} 
     x2={line} 
     y1={line} 
     y2={line} 
     stroke="black" 
     stroke-width={sw} />
     <line id="right" 
     x1={line} 
     x2={line} 
     y1={base} 
     y2={line} 
     stroke="black" 
     stroke-width={sw} />
     <line id="top" 
     x1={base} 
     x2={line} 
     y1={base} 
     y2={base} 
     stroke="black" 
     stroke-width={sw} />
     <line id="" 
     x1={base} 
     x2={line} 
     y1={base} 
     y2={line} 
     stroke="black" 
     stroke-width={sw} />
     <!-- 
     <line {x1} x2={x1+l} {y1} y2={y1} stroke="black" stroke-width="3"/>
     <line x1={x1} x2={x1} {y1} y2={y1+l} stroke="black" stroke-width="3"/>
     <line {x1} x2={x1+l} {y1} y2={y1} stroke="black" stroke-width="3"/>
       <line x1={base} x2="50" y1="110" y2="110" stroke="black" stroke-width="3"/>
     <line x1={base} x2="50" y1="110" y2="110" stroke="black" stroke-width="3"/>
     <line x1={base} x2="50" y1="110" y2="110" stroke="black" stroke-width="3"/>
     <line x1={base} x2="50" y1="110" y2="110" stroke="black" stroke-width="3"/> -->

  <!-- <rect width="100%" height="100%" fill="red" />

  <circle cx="150" cy="100" r="80" fill="green" />

  <text x="150" y="125" font-size={line} text-anchor="middle" fill="white">SVG</text> -->

</svg>
