<script>
let count = 0;

function handleIncrement() {
    count += 1;
}
function handleDecrement() {
    count -= 1;
}
function handleReset() {
    count = 0;
}
</script>
<br>
<div id="compteur-clics">
<div>
    <div>
    <input bind:value={count} type="number" id="count" />
    </div>

    <div>
    <button id="clics-plus" on:click={handleIncrement}>+</button>
	<button id="clics-moins" on:click={handleDecrement}>−</button>
    </div>
    
</div>
<div>
    <div>
    <button id="reset" on:click={handleReset}>reset</button>
    </div>
</div>
</div>

<style>
	#compteur-clics{
		width: 500px;
        margin: 0 auto;
        text-align: center;
		padding: 20px;
		background-color: rgb(190, 190, 190);
	}
	input{
		width: 450px;
		text-align: center;
	}
	#clics-plus{
		width: 225px;
		height: 55px;
		color: white;
		background-color: rgb(72, 129, 190);
	}
	#clics-moins{
		width: 225px;
		height: 55px;
		color: white;
		background-color: rgb(72, 129, 190);
	}
	#reset{
		width: 120px;
		border-color: red ;
		color: red;
	}
</style>