<template>
  <section class="frequently-asked-questions">
    <h3>Frequently asked questions</h3>
	<div class="faq">
		<a id="hide1" href="#hide1" class="hide">
			Praesent fermentum posuere varrius? 
			<span class="faq-icon"><img alt="Quickbooks logo" width="10px" src="@/assets/caret-down-solid.svg"></span>
		</a>
		<a id="show1" href="#show1" class="show">
			Praesent fermentum posuere varrius? 
			<span class="faq-icon"><img alt="Quickbooks logo" width="10px" src="@/assets/caret-up-solid.svg"></span>
		</a>
		<div class="details">
			Content goes here.
		</div>
	</div>
	<div class="faq">
		<a id="hide2" href="#hide2" class="hide">
			Integer semper efficitur lacus, nec semper lectus tempus id? 
			<span class="faq-icon"><img alt="Quickbooks logo" width="10px" src="@/assets/caret-down-solid.svg"></span>
		</a>
		<a id="show2" href="#show2" class="show">
			Integer semper efficitur lacus, nec semper lectus tempus id? 
			<span class="faq-icon"><img alt="Quickbooks logo" width="10px" src="@/assets/caret-up-solid.svg"></span>
		</a>
		<div class="details">
			Content goes here.
		</div>
	</div>
	<div class="faq">
		<a id="hide3" href="#hide3" class="hide">
			Sed erat dolor, pellentesque eu pulvinar eget, finibus at arcu? 
			<span class="faq-icon"><img alt="Quickbooks logo" width="10px" src="@/assets/caret-down-solid.svg"></span>
		</a>
		<a id="show3" href="#show3" class="show">
			Sed erat dolor, pellentesque eu pulvinar eget, finibus at arcu? 
			<span class="faq-icon"><img alt="Quickbooks logo" width="10px" src="@/assets/caret-up-solid.svg"></span>
		</a>
		<div class="details">
			Content goes here.
		</div>
	</div>
	<div class="faq">
		<a id="hide4" href="#hide4" class="hide">
			Praesent sollicitudin mauris a mattis tincidunt? 
			<span class="faq-icon"><img alt="Quickbooks logo" width="10px" src="@/assets/caret-down-solid.svg"></span>
		</a>
		<a id="show4" href="#show4" class="show">
			Praesent sollicitudin mauris a mattis tincidunt? 
			<span class="faq-icon"><img alt="Quickbooks logo" width="10px" src="@/assets/caret-up-solid.svg"></span>
		</a>
		<div class="details">
			Content goes here.
		</div>
	</div>
  </section>
</template>

<script>
export default {
  name: 'FrequentlyAskedQuestions',
	data() {
		return {
		}
	}
}
</script>

<style scoped>
.details,
.show,
.hide:target {
  display: none;
}
.hide:target + .show,
.hide:target ~ .details {
  display: block;
}

.frequently-asked-questions {
	margin-top: 40px;
    width: 80%;
}

.faq {
	border-bottom: 1px solid #eceef1;
	padding: 10px 0;
}

.faq a {
	margin-left: 40px;
	text-decoration: none;
	font-size: 12px;
	color: #000;
	font-weight: 200;
}

.faq-icon {
    float: right;
	margin-right: 20px;
}

.details {
	margin-left: 40px;
	font-size: 12px;
}

h3 {
  font-weight: bold;
  font-size: 20px;
  margin-left: 40px;
}

</style>