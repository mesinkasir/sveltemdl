<script>  
	import Beranda from "./Beranda.svelte";
	import Start from "./Start.svelte";
	import About from "./About.svelte";
	import Gallery from "./Gallery.svelte";
	import Pricing from "./Pricing.svelte";
	import Contact from "./Contact.svelte";
	export let menu = 1;
</script>
<div class="mdl-layout mdl-js-layout mdl-layout--fixed-header">
	<header class="mdl-layout__header bg-success">
	  <div class="mdl-layout__header-row">
		<span class="mdl-layout-title"><img width="120" class="img-fluid" alt="android" src="https://1.bp.blogspot.com/-Q_XwbXyx1K8/YXLFAMOloCI/AAAAAAAARa0/gkI51CDRc-8IoY8LL0_BObveIxAPkalVwCLcBGAsYHQ/s280/android-logo.png"/></span>
		<div class="mdl-layout-spacer"></div>
      <nav class="mdl-navigation mdl-layout--large-screen-only">
        <a class="mdl-navigation__link" href="https://wa.me/6285646104747"><span class="material-icons">
			whatsapp
			</span> Whatsapp</a>
        <a class="mdl-navigation__link" href="tel:+6285331361404"><span class="material-icons">
			call
			</span> Call Us</a>
        <a class="mdl-navigation__link" href="mailto:axcora@gmail.com"><span class="material-icons">
			alternate_email
			</span> Email</a>
      </nav>
    </div>
  </header>
  <div class="mdl-layout__drawer">
    <span class="mdl-layout-title p-3 bg-success text-center"><img class="img-fluid rounded-circle" width="120" alt="android" src="https://1.bp.blogspot.com/-9AUfrfEBePw/YXLNcfM2kAI/AAAAAAAARbY/Zw9LmLV-fFMAjUX6HUExuwTIZBdxPu7tACLcBGAsYHQ/s225/pembuatan%2Bandroid%2Baplikasi%2Bmurah.png"/>
	</span>
    <nav class="mdl-navigation">
      <a class="mdl-navigation__link" href="/" on:click|preventDefault={() => (menu = 1)}><span class="material-icons">home</span> Home</a>
			<a class="mdl-navigation__link" href="/" on:click|preventDefault={() => (menu = 2)}><span class="material-icons">android</span> About</a>
			<a class="mdl-navigation__link" href="/" on:click|preventDefault={() => (menu = 3)}><span class="material-icons">smartphone</span> Get Start</a>
			<a class="mdl-navigation__link" href="/" on:click|preventDefault={() => (menu = 4)}><span class="material-icons">insert_photo</span> Themes</a>
			<a class="mdl-navigation__link" href="/" on:click|preventDefault={() => (menu = 5)}><span class="material-icons">monetization_on</span> Pricing</a>
			<a class="mdl-navigation__link" href="/" on:click|preventDefault={() => (menu = 6)}><span class="material-icons">support_agent</span> Contact</a>
	
			<a class="mdl-navigation__link btn btn-dark" href="https://github.com/mesinkasir/sveltemdl/">
			  <strong>Github →</strong>
			</a>
    </nav>
  </div>
  <main class="mdl-layout__content">
    <div class="page-content"> 
{#if menu === 1}
<Beranda />
{:else if menu === 2}
<About />
{:else if menu === 3}
<Start />
{:else if menu === 4}
<Gallery />
{:else if menu === 5}
<Pricing />
{:else if menu === 6}
<Contact />
{:else}
<h1>
	404 Page Not Found
</h1>
{/if}
</div>
</main>
</div>

