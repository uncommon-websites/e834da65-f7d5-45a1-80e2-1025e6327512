<script lang="ts">
	// Types
	import type { PageProps } from "./$types";

	// Components
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import Pricing from "$lib/components/layout/Pricing.svelte";

	// Props
	const { data }: PageProps = $props();
</script>

<Pricing />

<Testimonials
	testimonials={[
		{
			name: "Suki Tanaka",
			position: "Founder",
			company: "Compli",
			quote:
				"We launched faster, saved money, and looked like a million-dollar company on day one. For any early team, it's a no-brainer.",
			image: "/generated/image-a-portrait-of-an-asian-woman-exuding-con.webp"
		},
		{
			name: "Elliott Maher",
			position: "Head of Product",
			company: "Gainlight",
			quote:
				"We didn't have a designer. We did have tight deadlines. This platform bridged that gap effortlessly and helped us raise our pre-seed.",
			image: "/generated/image-a-portrait-of-a-caucasian-man-embodying-.webp"
		},
		{
			name: "Mari Sanchez",
			position: "Operations Lead",
			company: "NodeOne",
			quote:
				"It felt like adding a design team overnight, without the overhead. We got polished outputs in hours, not weeks.",
			image: "/generated/image-a-portrait-of-a-hispanic-woman-showcasin.webp"
		},
		{
			name: "Dev Patel",
			position: "CEO",
			company: "MacroForge",
			quote:
				"It handles so many startup pain points with elegance and speed. Our deck, branding, and first site all came from here—and they held up under investor scrutiny.",
			image: "/generated/image-a-portrait-of-a-south-asian-man-reflecti.webp"
		}
	]}
/>

<CallToAction 
	title="Ready to transform your startup?"
	subtitle="Start your AI design journey today"
	description="Join thousands of successful startups who have accelerated their growth with our AI design solutions. Get professional designs in hours, not weeks, and focus on what matters most - building your business."
	imageSrc="/generated/image-a-joyful-startup-founder-with-an-express.webp"
	callsToAction={[
		{
			href: "/get-started",
			label: "Start free trial",
			variant: "primary"
		},
		{
			href: "/contact",
			label: "Schedule demo",
			variant: "secondary"
		}
	]}
/>
