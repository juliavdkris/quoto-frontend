<script>
    import Header from './components/Header.svelte';
    import Footer from './components/Footer.svelte';
</script>

<style>
    main {
        min-height: 100vh;

        display: flex;
	    flex-direction: column;

        color: #333;
    }

    .content {
        flex: 1;
    }
</style>

<main>
    <Header/>
    <div class="content"></div>
    <Footer/>
</main>