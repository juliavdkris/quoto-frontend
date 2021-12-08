
<!---------- Script ---------->

<script>

    import Navbar from '../components/Navbar.svelte';
    import Footer from '../components/Footer.svelte';

</script>

<!---------- Style ---------->

<style>

    main {
        min-height: 100vh;

        display: flex;
	    flex-direction: column;

        color: #333;
    }

    .content {
        padding: 2rem 3rem 5rem;
        flex: 1;

        display: flex;
    }

</style>

<!---------- Main code ---------->

<main>
    <div class="content">
        <Navbar/>
        <slot/>
    </div>
    <Footer/>
</main>