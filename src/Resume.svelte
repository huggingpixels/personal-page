<script>
    import Duck from "./assets/Duck.svelte";
</script>

<style>
    #pond {
        height: 200px;
    }

    #duck {
	    transform: translate(0px, 15px);
        animation: float 10s ease infinite;
        position: absolute;
    }
  
    @keyframes float {
	    0% {
	    	transform: translate(-50px, 15px);
        }
        25% {
	    	transform: translate(200px, 0px) scale(0.8);
        }
        50% {
	    	transform: translate(450px, 15px);
	    }
	    75% {
	    	transform: translate(700px, 0px) scale(0.8);
        }
	    100% {
		    transform: translate(950px, 15px);
	    }
    }
</style>

<h3 id="resume">Catch a duck to check my linkedin page</h3>
<div id="pond">
    <span id="duck"><Duck /></span>
</div>