<svelte:head>
  <title>Welcome</title>
 <style>
   @import url('https://fonts.googleapis.com/css2?family=Hurricane&family=Inspiration&family=Special+Elite&display=swap');
h1, ul, li, a {
        font-family: "Special Elite", cursive;
    }
    p {
        font-family: "Special Elite", sans-serif;
}
ul {
  list-style: none;
  margin: 10;
  padding: 10;
}
     body{
            background-color: #F5E6E9;
          }
 body.dark-mode {
		background-color: #1d3040;
		color: #bfc2c7;
	}
</style>
</svelte:head>
<h1 class="text-3xl font-bold underline">Christopher Patrouch</h1>
<Button>
	Toggle
</Button>
 <script>
   	import Button from './Button.svelte'
  	import profilepic from '$lib/images/profilepic2020.webp';
	let name = 'CPatraldo';
</script>
<p>tl;dr</p>
<p>My tools and current technology stack:</p>
<ul class="pl-2, text-2xl, list-disc list-inside"><li>Chromebook, with GNU/Linux enabled</li>
<li class="pl-4">Google Cloud</li>
</ul> 
<a href="javascript:alert('Hello {name.toUpperCase()}!');">Execute JavaScript</a>
<!--Div that will hold the pie chart-->
<p>
Send me an email: <a href="mailto:christopher@patrouch.dev">
<img alt="{name} is smiling" src={profilepic} border-width="10" width="200" height="200"/>
</a>
</p>

