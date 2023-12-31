<script>
	import { onMount } from 'svelte';
	import '../styles/global.css';
	import { afterNavigate } from '$app/navigation';
	import Nav from '../components/Nav.svelte';
	import Hero from '../components/Hero.svelte';
	import Features from '../components/Features.svelte';
	import Contact from '../components/Contact.svelte';
	import Footer from '../components/Footer.svelte';
	import Review from '../components/Review.svelte';
	import Faq from '../components/Faq.svelte';
	import About from '../components/About.svelte';

	afterNavigate(() => {
		HSStaticMethods.autoInit();
	});
</script>

<Nav />
<Hero />
<About />
<Features />
<Review />
<Faq />
<Contact />
<Footer />
