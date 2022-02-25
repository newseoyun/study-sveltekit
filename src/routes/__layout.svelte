<script>
    import Topbar from '$lib/Topbar.svelte'
</script>

<header>
    <Topbar />
</header>

<main>
    <slot><!-- optional fallback --></slot>
</main>

<footer>
    <p>Copyright 2022 Seoyun</p>
</footer>