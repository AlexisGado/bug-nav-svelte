<script>
    import { goto, pushState } from '$app/navigation';

    function submit() {
        pushState('/page1?a=1', {});
        goto('/page2?a=1');
    }
</script>
<a href="/">home</a>
<p>page1</p>
<button on:click={() => submit()}>Lez go</button>