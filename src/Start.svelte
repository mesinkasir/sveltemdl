<script>
	import Footer from "./widget/Footer.svelte";
	import Card1 from "./card/Card1.svelte";
	import Card2 from "./card/Card2.svelte";
	import Cards from "./card/Cards.svelte";
	import Card3 from "./card/Card3.svelte";
	import Cardvd from "./card/Cardvd.svelte";
	import Cardvs2 from "./card/Cardvs2.svelte";
</script>
<div class="row p-1">
	<div class="col-12 col-md-4 p-3">
	  <Cards/>
	  </div>
	  <div class="col-12 col-md-8 p-3">
		<Cardvd/>
	</div>
	<div class="col-12 col-md-4 p-3">
		<Card1/>
  </div>
  <div class="col-12 col-md-4 p-3">
	<Card2/>
	</div>
  <div class="col-12 col-md-4 p-3">
	<Card3/>
	</div>
	<div class="col-12 col-md-12 p-3">
		<Cardvs2/>
	</div>
</div>
  
<Footer/>