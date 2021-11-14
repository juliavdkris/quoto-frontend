
<!---------- Script ---------->

<script>

    import { slide } from 'svelte/transition';

    var dropdown = false;
    
    function clickOutside(element, callbackFunction) {
		function onClick(event) {
			if (!element.contains(event.target)) {
				callbackFunction();
			}
		}
		
		document.body.addEventListener('click', onClick);
		
		return {
			update(newCallbackFunction) {
				callbackFunction = newCallbackFunction;
			},
			destroy() {
				document.body.removeEventListener('click', onClick);
			}
		}
	}

</script>

<!---------- Style ---------->

<style>

    .menu-wrapper {
        width: 20rem;
    }

    .nav-wrapper {
        width: 100%;

        display: flex;
        align-items: stretch;
    }

    h1 {
        width: 100%;
        margin: 1rem 0;

        font-size: 3rem;
    }

    nav {
        margin: 0.5rem 0;
        flex: 1;

        display: flex;
        flex-direction: column;
    }

    a, button {
        margin-right: 1rem;
        padding: 0.875rem;

        border: none;
        background: none;
        text-align: left;
        text-decoration: none;
        font-family: inherit;
        font-size: inherit;
        color: inherit;
    }

    a:hover, button:hover {
        background-color: #eee;
    }

    .dropdown {
        display: flex;
        flex-direction: column;
    }

    .dropdown a {
        padding-left: 3rem;
    }

    .spacer {
        width: 3px;
        border-radius: 5px;
        background-color: #0E7C7B;

        animation: growVerticaly 1.5s ease-out 0.5s forwards;
        transform-origin: top;
        transform: scaleY(0);
    }

    @keyframes growVerticaly {
        100% { transform: scaleY(100%); }
    }

</style>

<!---------- Main code ---------->

<div class="menu-wrapper">
    <h1>Quotobot</h1>

    <div class="nav-wrapper">
        <nav>
            <a href="#">Home</a>
            <a href="#">About</a>
            <a href="#">Statistics</a>
            <div class="dropdown" use:clickOutside={ () => { dropdown = false; } }>
                <button on:click={ () => { dropdown = !dropdown; } }>Resources</button>
                {#if dropdown}
                    <a href="#" transition:slide>Documentation</a>
                    <a href="#" transition:slide>Github</a>
                {/if}
            </div>
        </nav>

        <div class="spacer"></div>
    </div>
</div>