<script lang="ts">
    import Card from '../components/Card.svelte';
</script>

<div class="max-w-svw min-h-screen p-2 grid gap-2 lg:grid-cols-3 lg:auto-rows-fr">
    <Card>
            <img src="logo.png" alt="CloakMind logo" class="h-64">
            <h1 class="eagle-lake text-5xl mt-2">CloakMind</h1>
    </Card>
    
    <Card>
        <span>
            A tiny non-corporate run by
            <!-- two Product Engineers:  -->
            <a href='https://shivangagr.netlify.app' target="_blank" class="eagle-lake accent link">
                Shivang
            </a>, and
            <a href='https://mitulagr.vercel.app' target="_blank" class="eagle-lake accent link">
                Mitul
            </a>
        </span>
    </Card>
    
    <Card>
        <span class="font-bold text-xl">
            For the builders. By the builders.
            <!-- We ask questions. -->
            <!-- We ask questions, we build, we break, we learn, we share. -->
        </span>
    </Card>
    
    <Card>
        <img src="deepseekret.svg" alt="DeepSeekret logo" class="h-24 m-4">
        <span class="max-w-sm">Keep your chats a
            <!-- <span class="font-bold text-transparent bg-gradient-to-r from-[#FCD400] to-[#C59A34] bg-clip-text"> -->
            <span class="font-bold">
                DeepSeekret
            </span>.
            <br />
            Secure, open-source, and free.
        </span>
        <a href='https://cloakmind.github.io/deepseekret' target="_blank" class="mt-4 p-1 pl-4 pr-4 text-sm font-semibold border-2 rounded-full">
            Learn more
        </a>
    </Card>
    
    <Card>
        <img src="logo.png" alt="DeepSeekret logo" class="h-24 m-4">
        <span>AgentCrest</span>
        <span class="mt-2 text-sm text-[#999] rounded-full">Coming soon</span>
    </Card>
    
    <Card>
        <span class="max-w-md text-sm">
            If you’re enjoying Daily,
            <a href='https://github.com/CloakMind' class="link">follow us</a> to be first to know what’s next.
            This site runs on Svelte.
            <a href='https://cloakmind.github.io' class="link">Learn how</a> to make one too.
        </span>
    </Card>
</div>

<style>
    /* .deepseekret { color: #FCD400; } */
</style>