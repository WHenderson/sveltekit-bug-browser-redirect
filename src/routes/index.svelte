<script context="module">
    import {browser} from "$app/env";

    export async function load() {
        if (browser) {
            // Note there would normally be some condition logic here
            return {
                status: 303,
                redirect: '/redirected',
            };
        }

        return {};
    }
</script>
<h1>Woops!</h1>
<p>You shouldn't be here. You should have been directed to /redirect!</p>
