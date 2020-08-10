<script lang="ts">

</script>

<style type="text/scss">
  main {
		position: relative;		
		
    svg {
			position: absolute;
			top: 100px;
			left: 100px;
      path {
        stroke: #ff00ff;
        stroke-width: 1px;
      }
    }
  }
</style>

<main>
  <svg width="500" height="500">
		<path fill="none" d="
			M 50,50
			C 50,50
			50,100  
			100,100" /> 
		<path fill="none" d="
			M 100,100 
			C 100,100
			150, 100  
			150,50" />
		<path fill="none" d="
			M 150,50     
			C 150,50
				150, 0
				100, 0" />
		<path fill="none" d="
			M 100,0     
			C 100,0
				50, 0
				50, 50" />	
  </svg>
</main>
