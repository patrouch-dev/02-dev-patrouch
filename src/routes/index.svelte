<svelte:head>
  <title>Welcome</title>
 <style>
   @import url('https://fonts.googleapis.com/css2?family=Hurricane&family=Inspiration&family=Special+Elite&display=swap');
 h1 {
        font-family: "Special Elite", cursive;
    }
    p {
        font-family: "Special Elite", sans-serif;
}
     body {
            background-color: #F5E6E9;
          }
</style>


</svelte:head>

<h1>Christopher Patrouch</h1>

 <script>
	let src = '/src/images/profilepic2020.webp';
	let name = 'CPatraldo';
</script>



<p>tl;dr
My tools and current technology stack, not necessarily by order:</p>
<ul><li>Chromebook, with GNU/Linux enabled</li>
<li>Google Cloud</li>
</ul> 
<a href="javascript:alert('Hello {name.toUpperCase()}!');">Execute JavaScript</a>

<p>
Send me an email: <a href="mailto:christopher@patrouch.dev">
<img {src} alt='{name} is smiling' border="10"  width="200" height="200">
</a>
</p>

