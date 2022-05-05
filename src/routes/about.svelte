<svelte:head>
<title>About</title>

<style>
@import url('https://fonts.googleapis.com/css2?family=Marmelad&family=Pacifico&family=Special+Elite&family=Tangerine:wght@400;700&family=Ultra&display=swap');
    h1 {
        font-family: "Special Elite", cursive;
    }     

 p {
       font-family: 'Marmelad', sans-serif;
color: purple;

    }
    

    body {
        background-color: #af875f;
    }	
        
</style>
</svelte:head>
<h1>about patrouch.dev</h1>
<script>
import Nested from './Nested.svelte';
	let string = `this string contains some <strong>HTML!!!</strong>`;

	let count = 0;


	function incrementCount() {
		count += 1;
                
	}

</script>

<button on:click={incrementCount}>
	Clicked {count} {count === 1 ? 'time' : 'times'}
</button>

<p>{@html string}</p>
<Nested/>


<p>This website is built with Sveltekit. It is served from an off-premise virtual server (Ubuntu) on Google Compute Engine. Nginx is configured for these purposes as a reverse proxy with an upstream directive. Other technologies used for this website are Node, PM2, and Letsencrypt. The DNS is managed through Google Domains. The local development machine is an HP Chromebook (8GB ram, 64GB storage, Intel M3 -- with GNU/Linux enabled. This website uses Google Analytics and possibly other tracking software and for that reason (and certainly many more reasons) this site is not compliant with basic user freedoms the way it ought be. For more information on technology's destruction of your freedom, start here: <a href="http://fsf.org">Free Software Movement</a></p>  
<style>

h1 {
        font-family: "Special Elite", cursive;
    }
p {
       font-family: 'Marmelad', sans-serif;
color: black;
       font-size: 2em;
    }
</style>
