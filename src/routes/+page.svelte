<script>
	import FeaturedArticle from './FeaturedArticle.svelte';
	import Article from './Article.svelte';

	import featuredImage from '$lib/assests/featuredArticle/main.jpg';
    import sfllImage from '$lib/assests/sfll/main.jpg';
    import dynamicBookmarkImage from '$lib/assests/dynamicBookmarks/main.png';
</script>

<div>
	<FeaturedArticle
		tag="meta"
		image={featuredImage}
		title="A blog, yay!"
		summary="Introducing my blog. It is built with svelte. Here i will document and showcase my creative work."
	/>

	<span id="latest">Latest Articles</span>
	<div class="grid grid-cols-1 md:grid-cols-2 gap-4 md:gap-8">
		<Article
			tag="salesforce"
			image={sfllImage}
			title="SFLL, A script to re-authenticate salesforce orgs in VS Code"
			summary="sfdx-cli often fails to authenticate with orgs. And we have to authenticate the same org again. sfll automates this re-authentication. Here i document process of creating this script."
		/>

		<Article
			tag="meta"
			image={dynamicBookmarkImage}
			title="Dynamic bookmarks to quickly navigate salesforce orgs"
			summary="We often hop between setup, object-manager, developer-console and any particular app in salesforce orgs. What if i told you, there is a way to bookmark these 4 horsemen, bookmarks which will work across any salesforce org!"
		/>
	</div>
</div>

<style>
	#latest {
		font-size: 46px;
		line-height: 50px;
		letter-spacing: -0.5px;
        /* font-family: 'Ubuntu Mono', monospace; */
        display: block;
        margin-top: 60px;
        margin-bottom: 30px;
        
	}

	@media (max-width: 1280px) {
		#latest {
			font-size: 22px;
			line-height: 26px;
			letter-spacing: -0.5px;
            /* font-family: 'Ubuntu Mono', monospace; */
		}
	}
</style>
