<script lang="ts">
	const items = [
		{ title: 'Home', href: '/' },
		{ title: 'About', href: '/about' }
	];
</script>

<nav class="main-nav">
	<div>Hako</div>
	<div class="nav-items">
		{#each items as { title, href }}
			<a class="nav-link" {href}>{title}</a>
		{/each}
	</div>
    <div>
        switch
    </div>
</nav>

<style>
	.main-nav {
        box-sizing: border-box;
        width: 100%;
        height: 60px;
        padding: 0 40px;

		display: flex;
		align-items: center;
		justify-content: space-between;

        position: fixed;
        top: 0;
        left: 0;
	}

    .nav-items {
        display: flex;
        gap: 12px;
    }

    .nav-link {
        font-weight: bold;
    }

    .nav-link:hover {
        color: blue;
    }
</style>
