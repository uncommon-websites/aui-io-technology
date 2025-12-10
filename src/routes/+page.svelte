<script lang="ts">
	import Header from "$lib/components/Header.svelte";
	import Hero from "$lib/components/Hero.svelte";
	import FeatureHighlight from "$lib/components/FeatureHighlight.svelte";
	import TextSection from "$lib/components/TextSection.svelte";
	import FeaturesGrid from "$lib/components/FeaturesGrid.svelte";
	import ComparisonSection from "$lib/components/ComparisonSection.svelte";
	import UnderstandingSection from "$lib/components/UnderstandingSection.svelte";
	import ComparisonTable from "$lib/components/ComparisonTable.svelte";
	import SafetySection from "$lib/components/SafetySection.svelte";
	import Footer from "$lib/components/Footer.svelte";
</script>

<main class="bg-background min-h-screen text-white selection:bg-accent selection:text-white overflow-x-hidden">
	<Header />
	<Hero />
	<FeatureHighlight />
	<TextSection />
	<FeaturesGrid />
	<ComparisonSection />
	<UnderstandingSection />
	<ComparisonTable />
	<SafetySection />
	<Footer />
</main>

