<script>
    import Header from './components/Header.svelte';
    import Navbar from './components/Navbar.svelte';
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
        padding: 5rem 2rem;
    }
</style>

<main>
    <Header/>
    <div class="content">
        <Navbar/>
    </div>
    <Footer/>
</main>