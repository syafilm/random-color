<script>
	let count = 0;

	function handleClick() {
	  let x = document.querySelector("body");
	  let r = Math.round(Math.random(255) * 255);
	  let g = Math.round(Math.random(255) * 255);
	  let b = Math.round(Math.random(255) * 255);
	  let ranCol = `rgb(${r}, ${g}, ${b})`;
	  x.style.backgroundColor = ranCol;

	  let text = document.querySelector("p");
	  text.innerHTML = ranCol;
	}
</script>

<style>
	button {
	  background: white;
	  color: #333;
	  border: none;
	  padding: 8px 12px;
	  border-radius: 2px;
	  margin-top: 240px;
	  font-weight: bold;
	  font-size: 1.5rem;
	}
	p {
	  width: max-content;
	  margin: 1rem auto;
	  background: white;
	  color: #333;
	  border: none;
	  padding: 8px 12px;
	  border-radius: 2px;
	  font-weight: bold;
	  font-size: 1.5rem;
	}
</style>

<button on:click={handleClick}>
  Click me
</button>

<p>rgb(255, 255, 255)</p>