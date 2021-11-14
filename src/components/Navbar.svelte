<style>

    .nav-wrapper {
        width: 20rem;
        display: flex;
        align-items: stretch;
    }

    nav {
        margin: 0.5rem 0;
        flex: 1;

        display: flex;
        flex-direction: column;
    }

    nav a {
        margin-right: 1rem;
        padding: 0.875rem;

        text-decoration: none;
        color: inherit;
    }

    nav a:hover {
        background-color: #eee;
    }

    .spacer {
        width: 3px;
        border-radius: 5px;
        background-color: #0E7C7B;

        animation: growVerticaly 1s ease-out 0.5s forwards;
        transform-origin: top;
        transform: scaleY(0);
    }

    @keyframes growVerticaly {
        0%   { 
            transform: scaleY(0);
        }
        100% {
            transform: scaleY(100%);
        }
    }

</style>

<div class="nav-wrapper">
    <nav>
        <a href="#">Home</a>
        <a href="#">Blog</a>
        <a href="#">About</a>
        <a href="#">Resources</a>
        <a href="#">Statistics</a>
    </nav>

    <div class="spacer"></div>
</div>