<script lang="ts">
    import Nav from '../components/Nav.svelte';
    import type { LayoutProps } from './$types';

    let { children }: LayoutProps = $props();
</script>

<header>
    <Nav />
</header>
<main class="container">
    {@render children()}
</main>
<footer class="footer">
    &copy; ave mujica
</footer>

<style>
    .container {
        flex: 1;

        box-sizing: border-box;
        padding-top: 60px;
        width: 100%;
        max-width: 960px;

        margin: 0 auto;
    }

    .footer {
        text-align: center;

        padding: 40px 0;
    }
</style>