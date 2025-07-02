<script lang="ts">
	// Types

	// Components
	import SectionHeader from "$lib/components/layout/SectionHeader.svelte";
	import Culture from "$lib/components/layout/Culture.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import SecondaryHero from "$lib/components/layout/hero-sections/SecondaryHero.svelte";
	import Card from "$lib/components/ui/Card.svelte";
	import JobList, { type JobOpening } from "./JobList.svelte";

	// Icons
	import IconBriefcase from "~icons/lucide/briefcase";
	import IconUsers from "~icons/lucide/users";
	import IconHeart from "~icons/lucide/heart";
	import IconGlobe from "~icons/lucide/globe";

	// Constants
	const SECTION_BASE_CLASSES = "section-py section-px container mx-auto";
	const GRADIENT_BG_CLASSES =
		"bg-gradient-to-br from-gray-50 to-gray-100 dark:from-gray-900 dark:to-gray-800";
	const ICON_CONTAINER_CLASSES =
		"bg-primary-50 text-primary-600 dark:bg-primary-950 dark:text-primary-400 flex items-center justify-center rounded-full";

	const benefits = [
		{
			title: "AI-First Innovation",
			description: "Work at the forefront of AI and design innovation, shaping how startups build their brands.",
			icon: IconBriefcase
		},
		{
			title: "Startup Growth Journey",
			description: "Experience exponential growth alongside our startup clients while developing cutting-edge AI design tools.",
			icon: IconUsers
		},
		{
			title: "Direct Impact",
			description: "See your work launch companies and transform startup dreams into reality through AI-powered design.",
			icon: IconHeart
		}
	];

	const openings: JobOpening[] = [
		// AI & Engineering
		{
			title: "AI Design Engineer",
			department: "AI & Engineering",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Machine Learning Engineer",
			department: "AI & Engineering",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Full-Stack Developer",
			department: "AI & Engineering",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},

		// Design
		{
			title: "Startup Design Strategist",
			department: "Design",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "AI-Powered Designer",
			department: "Design",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},

		// Product
		{
			title: "Product Manager - AI Tools",
			department: "Product",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Startup Success Manager",
			department: "Product",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},

		// Growth & Marketing
		{
			title: "Growth Marketing Manager",
			department: "Growth & Marketing",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Startup Community Manager",
			department: "Growth & Marketing",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Content Creator - AI Design",
			department: "Growth & Marketing",
			location: "Remote",
			type: "Full-time",
			url: "#"
		}
	];

	const employeeTestimonials = [
		{
			name: "Aisha Patel",
			position: "Senior AI Design Engineer",
			company: "Engineering Team",
			quote:
				"The technical challenges here constantly push me to develop cutting-edge AI solutions. Working alongside brilliant engineers while building tools that genuinely help startups succeed makes every sprint exciting.",
			image:
				"/generated/image-a-professional-headshot-of-a-south-asian.webp"
		},
		{
			name: "Marcus Thompson",
			position: "Product Growth Lead",
			company: "Product Team",
			quote:
				"I joined as a junior analyst and moved into product leadership within 18 months. The mentorship opportunities and direct startup exposure have accelerated my career beyond what I imagined possible.",
			image:
				"/generated/image-a-professional-headshot-of-a-black-man-p.webp"
		},
		{
			name: "Elena Rodriguez",
			position: "Junior Designer",
			company: "Design Team",
			quote:
				"As someone new to the industry, the supportive culture here has been incredible. Senior designers take time to guide my growth, and seeing my work help real founders launch their companies is incredibly motivating.",
			image:
				"/generated/image-a-professional-headshot-of-a-hispanic-wo.webp"
		}
	];

	const processSteps = [
		{
			step: 1,
			title: "Apply",
			description:
				"Submit your application with examples of AI/design work, startup experience, or passion projects that show your innovative thinking."
		},
		{
			step: 2,
			title: "AI Design Challenge",
			description: "Complete a brief design challenge using AI tools to demonstrate your problem-solving approach for startup scenarios."
		},
		{
			step: 3,
			title: "Team Collaboration",
			description: "Meet our AI design team to discuss startup challenges, share ideas, and explore how you'll contribute to founder success."
		},
		{
			step: 4,
			title: "Welcome Aboard",
			description: "Join our mission to democratize great design for startups and help build the next generation of successful companies."
		}
	];

	const values = [
		{
			icon: IconHeart,
			title: "Startup Mindset",
			description: "We think like entrepreneurs, move fast, and embrace the startup journey with passion and resilience."
		},
		{
			icon: IconUsers,
			title: "AI-Powered Creativity",
			description: "We blend artificial intelligence with human creativity to unlock new possibilities in design and company building."
		},
		{
			icon: IconGlobe,
			title: "Founder Success",
			description: "We measure our success by the startups we help launch and the founders whose dreams we help realize."
		}
	];
</script>

<!-- Hero Section -->

<SecondaryHero
	title="Shape the future of AI-powered design"
	subtitle="Join a passionate team building the next generation of design tools that empower startups to succeed. Create meaningful impact while advancing your career in an innovative, collaborative environment."
	imageSrc="/generated/image-a-modern-collaborative-workspace-with-a-.webp"
/>

<!-- Why Join Us Section -->
<section class={SECTION_BASE_CLASSES}>
	<SectionHeader title="Why join us?" subtitle="Shape the future of startup design with AI innovation" />

	<div class="mt-16 grid gap-4 md:grid-cols-3">
		{#each benefits as benefit}
			<Card {...benefit} />
		{/each}
	</div>
</section>

<!-- Culture Section -->
<Culture {values} />

<Testimonials testimonials={employeeTestimonials} />

<!-- Application Process -->
<section class={SECTION_BASE_CLASSES}>
	<div class="mx-auto">
		<h2 class="text-title1 mb-16">Our application process</h2>

		<div class="grid gap-12 md:grid-cols-2 lg:grid-cols-4">
			{#each processSteps as { step, title, description }, i}
				<div class="flex flex-col">
					<div class="{ICON_CONTAINER_CLASSES} mb-6 size-11">
						<span class="text-headline">{step}</span>
					</div>
					<h3 class="text-headline mb-3">{title}</h3>
					<p class="text-body text-emphasis-low">{description}</p>
				</div>
			{/each}
		</div>
	</div>
</section>
<!-- Current Openings Section -->
<section class={GRADIENT_BG_CLASSES}>
	<div class="section-px section-py container mx-auto grid w-full items-start lg:grid-cols-2">
		<SectionHeader title="Current openings" subtitle="Find your perfect role" />

		<JobList {openings} />
	</div>
</section>
