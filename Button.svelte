<script>
	let count = 0;
	const button = document.querySelector("button");

	function handleClick() {
	  count += 1;
	}
</script>

<style>
	button {
	  width: 110px;
	  background: #ff3e00;
	  color: white;
	  border: none;
	  padding: 8px 12px;
	  border-radius: 2px;
	}
	button:focus {
	  outline: none;
	  cursor: pointer;
	}
	button:hover {
	  cursor: pointer;
	}
</style>

<button on:click={handleClick}>
  Clicked {count} {count === 1 ? 'time' : 'times'}
</button>