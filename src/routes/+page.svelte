<script lang="ts">
	import ResponsiveImage from './ResponsiveImage.svelte';
</script>

<div class="wrapper">
	<section>
		<div>
			<h1>Hi my name is Zachiah!</h1>
			<div class="image-container">
				<ResponsiveImage src="/pfp.jpg" alt="A picture of Zachiah Sawyer" />
			</div>
		</div>
	</section>

    <section>
        <div></div>
    </section>
</div>

<style>
	:global(*) {
		box-sizing: border-box;
		padding: 0;
		margin: 0;
		font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode',
			Geneva, Verdana, sans-serif;
		font-size: 16px;
		font-weight: normal;
		color: currentColor;
		text-decoration: none;
	}

    .wrapper {
        scroll-snap-type: y mandatory;
        height: 100vh;
        overflow: auto;
    }

    h1 {
        font-size: 2rem;
        margin: 1rem 0;
    }
	section {
		height: 100%;
		width: 100vw;
		display: flex;
		align-items: center;
		justify-content: center;
        scroll-snap-align: start;
	}

	section > div {
		padding: 2rem;
        width: 50%;
        max-width: 100%;
	}
    
    .image-container {
    }
</style>
