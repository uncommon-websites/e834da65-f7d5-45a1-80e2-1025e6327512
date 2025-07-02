<script lang="ts">
	// Components
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import StakeholderGrid from "$lib/components/layout/StakeholderGrid.svelte";
	import Story from "./Story.svelte";
	import SecondaryHero from "$lib/components/layout/hero-sections/SecondaryHero.svelte";
	import Culture from "$lib/components/layout/Culture.svelte";

	// Constants
	const values = [
		{
			title: "AI-First Design",
			description: "Leveraging cutting-edge artificial intelligence to democratize professional design for every startup."
		},
		{
			title: "Founder Focused",
			description: "Understanding startup needs and building solutions that move at the speed of entrepreneurship."
		},
		{
			title: "Accessible Excellence",
			description: "Making studio-quality design affordable and effortless for teams of any size or budget."
		}
	];
</script>

<SecondaryHero
	title="Empowering startups with intelligent design"
	subtitle="Building the future of AI-powered company creation"
	imageSrc="/generated/image-a-diverse-group-of-people-collaborating-.webp"
/>

<!-- Story Section -->
<Story
	paragraphs={[
		"Most startup stories begin with a bold idea and not enough time, money, or people. We've been there. Hiring a professional designer felt out of reach, and even DIY tools added more confusion than clarity. That's why we built AI Designer for Startups—to give early-stage founders design support that feels like a real studio, but moves faster and costs way less.",
		"Our mission is to democratize great design. Every startup deserves to look polished and professional from day one. Whether you're building your first landing page, pitching investors, or launching a product—your visual identity matters. By using AI to replicate the workflows of top-tier design teams, we empower founders to create strong brand foundations without needing creative departments or painful design lessons.",
		"Here's our approach: understand what startups actually need, then simplify it using smart, scalable design systems. You don't have to speak in design terminology—we translate ideas into output that's clear, consistent, and crafted to grow with your company. Think brand visuals, pitch-ready decks, responsive landing pages, and marketing assets—all generated in minutes. No bottlenecks. No bloat. Just fast, founder-first design aligned to your startup's goals."
	]}
/>

<!-- Our Culture Section -->
<Culture {values} />

<!-- StakeholderGrid Section -->
<StakeholderGrid
	stakeholderType="team"
	title="Our team."
	subtitle="Your partners in innovation."
	stakeholders={[
		{
			name: "Alex Morgan",
			position: "Founder & CEO",
			bio: "Started the company with a vision to transform the industry through innovative solutions.",
			image:
				"https://images.unsplash.com/photo-1560250097-0b93528c311a?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=774&q=80"
		},
		{
			name: "Jamie Chen",
			position: "Chief Design Officer",
			bio: "Award-winning designer with a passion for creating intuitive and beautiful experiences.",
			image:
				"https://images.unsplash.com/photo-1573496359142-b8d87734a5a2?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=776&q=80"
		},
		{
			name: "Taylor Wright",
			position: "Head of Engineering",
			bio: "Technology enthusiast focused on building scalable systems that make a difference.",
			image:
				"https://images.unsplash.com/photo-1580489944761-15a19d654956?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=774&q=80"
		}
	]}
/>

<StakeholderGrid
	stakeholderType="investor"
	title="Backed by the best."
	subtitle="Point Nine, TSIC and others"
	stakeholders={[
		{
			name: "Point Nine Capital",
			image: "https://cdn.brandfetch.io/pointnine.com/w/400/h/400/logo?c=1id_elLz2Bd5Ej-dWo7"
		},
		{
			name: "TSIC Ventures",
			image: "https://cdn.brandfetch.io/tiny.vc/w/400/h/400/logo?c=1a2b3c4d5e"
		},
		{
			name: "Sequoia Capital",
			image: "https://cdn.brandfetch.io/sequoiacap.com/w/400/h/400/logo"
		}
	]}
/>

<!-- CTA Section -->
<CallToAction
	title="Ready to design smarter?"
	subtitle="Start building your brand today"
	description="Join hundreds of startups already using AI-powered design to launch faster, look professional, and focus on what matters most—building their business."
/>
