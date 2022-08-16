<script>
	function toggle() {
		window.document.body.classList.toggle('dark-mode')
	}
	</script>
	<button on:click={toggle}>
		<slot/>
	</button>
	<div class="bg-red-900 text-white">
		<h3 class="bg-red-600 text-red-900">Join our mailing list</h3>
		<div>
		  <p>Be the first to hear about our new offerings</p>
		  <button class="bg-red-600" type="button">Sign up</button>
		</div>
	  </div>
	<style>
		button {
			background-color: #294527;
			color: white;
			border: none;
			border-radius: 4px;
			padding: 0.5rem;
			text-transform: uppercase;
			
		}
		:global(body.dark-mode) button {
			background-color: darkolivegreen;
			color: white;
		}
	</style>