<!-- Change the GA ID before using this -->

<script>
  let analytics = true;

  if (process.env.NODE_ENV == "development") {
    analytics = false;
  }
</script>

<svelte:head>
  {#if analytics}
    <!-- Global site tag (gtag.js) - Google Analytics -->
    <script
      async
      src="https://www.googletagmanager.com/gtag/js?id=G-G17ZQ9KSG2"></script>
    <script>
      window.dataLayer = window.dataLayer || [];
      function gtag() {
        dataLayer.push(arguments);
      }
      gtag("js", new Date());

      gtag("config", "G-G17ZQ9KSG2");
    </script>
  {/if}
</svelte:head>
