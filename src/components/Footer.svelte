
<!-- Style -->
<style>
    
    ul {
        list-style: none;
        padding-left: 0;
    }

    footer {
        color: #bbb;
        background-color: #555;
        line-height: 1.5;
    }

    footer a {
        text-decoration: none;
        color: #bbb;
    }

    a:hover {
        color: #eee;
    }

    .footer-title {
        color: #fff;
        font-size: 1.3rem;
        padding-bottom: 0.625rem;
    }

    .footer-main {
        padding: 1.25rem 1.875rem;

        display: flex;
        flex-wrap: wrap;
    }

    @media only screen and (min-width: 29.8125rem) {
        .footer-main {
            justify-content: space-around;
        }
    }

    @media only screen and (min-width: 77.5rem) {
        .ft-main {
            justify-content: space-around;
        }
    }

    .footer-main-item {
        padding: 1.25rem;
        min-width: 12.5rem;
    }

    form {
        display: flex;
        flex-wrap: wrap;
    }

    input[type="text"] {
        margin-top: 0.3125rem;
        padding: 0.625rem;

        border: 0;
    }

    input[type="submit"] {
        margin-top: 0.3125rem;
        padding: 0.625rem 0.9375rem;

        background-color: #17bebb;
        color: #fff;
        cursor: pointer;
        border: 0;
    }

    .footer-legal {
        padding: 0.9375rem 1.875rem;
        background-color: #333;
    }
    
    .footer-legal-list {
        width: 100%;
        display: flex;
        flex-wrap: wrap;
    }

    .footer-legal-list li {
        margin: 0.125rem 0.625rem;
        white-space: nowrap;
    }

    .footer-legal-list li:nth-last-child(2) {
        flex: 1;
    }

</style>

<!-- Footer -->
<footer>

    <!-- Main footer -->
    <section class="footer-main">
        <div class="footer-main-item">
            <h2 class="footer-title">ABOUT</h2>
            <ul>
                <li><a href="#">Creators</a></li>
                <li><a href="#">Saffire</a></li>
                <li><a href="#">Discord</a></li>
            </ul>
        </div>
        <div class="footer-main-item">
            <h2 class="footer-title">NAVIGATION</h2>
            <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">Blog</a></li>
                <li><a href="#">Global Statistics</a></li>
                <li><a href="#">Server Statistics</a></li>
            </ul>
        </div>
        <div class="footer-main-item">
            <h2 class="footer-title">RESOURCES</h2>
            <ul>
                <li><a href="#">Docs</a></li>
                <li><a href="#">Github</a></li>
            </ul>
        </div>
        <div class="footer-main-item">
            <h2 class="footer-title">LOGIN</h2>
            <p>Login in to view server specific statistics.</p>
            <form>
                <input type="text" name="guild-id" placeholder="Enter Guild ID">
                <input type="submit" value="Login">
            </form>
        </div>
    </section>

    <!-- Legal footer -->
    <section class="footer-legal">
        <ul class="footer-legal-list">
            <li><a href="#">Terms &amp; Conditions</a></li>
            <li><a href="#">Privacy Policy</a></li>
            <li>&copy; 2021 Copyright Quotobot</li>
        </ul>
    </section>

</footer>