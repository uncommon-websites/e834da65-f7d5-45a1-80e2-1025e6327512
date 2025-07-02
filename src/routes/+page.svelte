<script lang="ts">
	// Components
	import UseCases from "$lib/components/layout/UseCases.svelte";
	import Summary from "$lib/components/layout/Summary.svelte";
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import AboutTeaser from "$lib/components/layout/AboutTeaser.svelte";
	import LogoScroller from "$lib/components/layout/LogoScroller.svelte";
	import Hero from "$lib/components/layout/hero-sections/Hero.svelte";
</script>

<Hero
	title="Design done for you"
	subtitle="Everything your startup needs to get started"
	imageSrc="/generated/image-a-group-of-diverse-startup-founders-cele.webp"
	centered={false}
/>
<LogoScroller 
	label="Trusted by innovative startups"
	logoUrls={[
		'https://logo.clearbit.com/stripe.com',
		'https://logo.clearbit.com/notion.so',
		'https://logo.clearbit.com/figma.com',
		'https://logo.clearbit.com/discord.com'
	]}
/>

<Summary
	title="What we do"
	text="We provide AI-powered design solutions specifically tailored for startups to accelerate their company building journey. Our platform offers intelligent design assistance across branding, websites, and marketing materials to help new businesses establish their professional presence. From logo creation to full brand identity development, we make high-quality design accessible and affordable for early-stage companies."
/>

<Testimonials
	testimonials={[
		{
			name: "Jordan Mehra",
			position: "Founder and CEO",
			company: "Streamcrate",
			quote:
				"We trimmed our design process from 3 months down to 2 weeks using AI Designer. It let us move forward without waiting on freelancers or burning budget.",
			image: "/generated/image-a-man-in-a-cozy-home-office-sitting-at-a.webp"
		},
		{
			name: "Zoe Kimani",
			position: "Cofounder",
			company: "SpindleSync",
			quote:
				"Our investor deck looked like a Series A pull—done overnight. It gave us a serious edge and made potential partners take us seriously despite being just 2 weeks old.",
			image: "/generated/image-a-woman-working-on-a-rooftop-workspace-d.webp"
		},
		{
			name: "Elias Rondo",
			position: "Cofounder",
			company: "BrambleHQ",
			quote:
				"We saved over $50,000 compared to agency quotes and still got branding strong enough to hold up in front of VCs. Dollar for dollar, nothing comes close.",
			image: "/generated/image-a-man-relaxing-in-a-modern-coworking-spa.webp"
		}
	]}
/>

<Features
	title="Everything your startup needs"
	subtitle="Professional design made accessible for early-stage companies"
	features={[
		{
			title: "Instant brand identity",
			description:
				"Generate logos, color palettes, and complete brand kits in seconds. No creative brief needed—just describe your startup vision."
		},
		{
			title: "Pitch deck ready assets",
			description:
				"Create investor-ready presentations and marketing materials. Turn rough ideas into polished, professional designs that impress stakeholders."
		},
		{
			title: "Website and landing pages",
			description:
				"Build conversion-focused web experiences without a developer. AI generates responsive designs optimized for your target audience."
		},
		{
			title: "No designer needed",
			description:
				"Access studio-quality design without hiring overhead. Perfect for pre-seed startups moving fast on limited budgets."
		},
		{
			title: "Edit like a document",
			description:
				"Customize every generated asset with intuitive editing tools. Make changes instantly—no complex design software required."
		},
		{
			title: "Startup speed delivery",
			description:
				"From concept to final assets in minutes, not weeks. Move as fast as your ideas without compromising on design quality."
		}
	]}
/>

<UseCases
	title="Use Cases"
	subtitle="Real-world applications for your business needs"
	useCases={[
		{
			title: "Launch with professional branding",
			description:
				"When starting your company, first impressions matter. Generate complete brand identities including logos, color palettes, and style guides that make investors and customers take you seriously from day one.",
			image: "/generated/image-a-startup-founder-is-sitting-at-a-modern.webp",
			link: {
				href: "/use-cases/brand-identity",
				label: "Learn more"
			}
		},
		{
			title: "Create investor-ready pitch decks",
			description:
				"Fundraising requires polished presentations that tell your story compelling. Our AI generates slide designs and layouts that help founders communicate their vision clearly to potential investors.",
			image: "/generated/image-an-entrepreneur-is-standing-in-front-of-.webp",
			link: {
				href: "/use-cases/pitch-decks",
				label: "See examples"
			}
		},
		{
			title: "Build conversion-focused websites",
			description:
				"Your website is often the first touchpoint with customers. Design and deploy professional landing pages and full websites that convert visitors into users without needing a development team.",
			image: "/generated/image-a-small-startup-team-is-gathered-around-.webp",
			link: {
				href: "/use-cases/websites",
				label: "View templates"
			}
		}
	]}
/>

<AboutTeaser />
<CallToAction />
