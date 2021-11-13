<script>
    import Footer from './components/Footer.svelte';
</script>

<style>
    main {
        min-height: 100vh;

        display: flex;
	    flex-direction: column;
    }

    .content {
        flex: 1;
    }
</style>

<main>
    <div class="content"></div>
    <Footer/>
</main>