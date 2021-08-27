<template>
  <div>
		<section class="hero is-success is-bold">
		<div class="hero-body">
				<p class="title">
				How To Play
				</p>
				<p class="subtitle">
				Setting up SRB2Kart to Join Kuu-Kart
				</p>
		</div>
	</section>
  <section class="section">
    <div class="container">
      <Content class="content"/>
    </div>
  </section>
  </div>
</template>

<script>
import Content from './assets/content.md'

export default {
  components: {
    Content
  },
  
  data() {
    return {
    }
  }
}
</script>