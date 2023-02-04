<script>
	export let image;
	export let tag = 'tag';
	export let title = 'Title';
	export let summary = 'Short description of for given title';

	let scaleOnHover = 'scale-100';
	let underlineClass = '';
	let arrowForwardOnHover = '';
	// image seed- https://www.freepik.com/free-vector/collection-watercolor-covers-pastel-colors_11481471.htm?query=abstract&collectionId=236&&position=34&from_view=collections
</script>

<a id="featuredArticle" href="#">
<div class="grid grid-cols-3" on:mouseenter={() => {scaleOnHover='scale-105'; underlineClass="underline"; arrowForwardOnHover='fill-blue-500 translate-x-4'}} on:mouseleave={() => {scaleOnHover='scale-100'; underlineClass=''; arrowForwardOnHover=''}}>
	<div class="col-span-3 xl:col-span-2 overflow-hidden rounded-xl xl:rounded-3xl" style="max-height: 450px;">
		<img src={image} class="duration-500 {scaleOnHover}"/>
	</div>

	<div class="col-span-3 xl:col-span-1 ml-0 mt-3 xl:ml-6">
		<div id="tag">{tag}</div>
		<div id="title" class="{underlineClass}">{title}</div>	
		<div id="summary">{summary}</div>
		<div class="flex flex-row-reverse pr-6 pt-2 xl:pt-6">
			<svg xmlns="http://www.w3.org/2000/svg" height="24" width="24" class="duration-300 {arrowForwardOnHover}">
				<path d="m12 20-1.425-1.4 5.6-5.6H4v-2h12.175l-5.6-5.6L12 4l8 8Z"/>
			</svg>
		</div>
	</div>
</div>
</a>


<style>
	#featuredArticle {
		display: block;
		margin-bottom: 32px;
	}

	#tag {
		/* font-family: 'Roboto Mono', monospace; */
		text-transform: lowercase;
		margin-bottom: 10px;
	}

	#title {
		font-size: 36px;
		font-weight: 400;
		line-height: clamp(36px, 3.06vw, 44px);
		margin-bottom: 25px;
		letter-spacing: -0.5px;
		/* font-family: 'Open Sans', sans-serif;	 */
	}

	#summary {
		font-size: 18px;
		font-weight: 100;
		
		margin-bottom: 25px;
		letter-spacing: -0.5px;
	}

	@media (max-width: 1280px) {
		#title {
			font-size: 30px;
			font-weight: 400;
			line-height: clamp(36px, 3.06vw, 44px);
			margin-bottom: 25px;
			letter-spacing: -0.5px;
		}
	}
</style>
