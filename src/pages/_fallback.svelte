
<!---------- Script ---------->

<script>

    import { url } from '@roxi/routify'

</script>

<!---------- Style ---------->

<style>

    .huge {
        font-size: 12rem;
    }
    .e404 {
        position: absolute;
        left: 50%;
        top: 50%;
        transform: translate(-50%, -50%);
        text-align: center;
    }

</style>

<!---------- Main code ---------->

<div class="e404">
    <div class="huge">404</div>
    <div class="big">
        <!-- link to the parent folder of _fallback.svelte -->
        Page not found.
        <a href={$url('../')}>Go back</a>
    </div>
</div>