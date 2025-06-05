<script lang="ts">
    import Card from '../components/Card.svelte';
</script>

<div class="grid min-h-screen max-w-svw gap-2 p-2 lg:auto-rows-fr lg:grid-cols-3">
    <Card>
        <img src="favicon.png" alt="CloakMind logo" class="h-64" />
        <h1 class="eagle-lake mt-2 text-5xl">CloakMind</h1>
    </Card>

    <Card>
        <span>
            A tiny non-corporate run by
            <!-- two Product Engineers:  -->
            <a
                href="https://shivangagr.netlify.app/?ref=cloakmind"
                target="_blank"
                class="eagle-lake accent link"
            >
                Shivang
            </a>, and
            <a
                href="https://mitulagr2.vercel.app/?ref=cloakmind"
                target="_blank"
                class="eagle-lake accent link"
            >
                Mitul
            </a>
        </span>
    </Card>

    <Card>
        <img src="pawss.png" alt="Pawss logo" class="m-4 h-24" />
        <span class="max-w-sm">
            Meet
            <!-- <span class="font-bold text-transparent bg-gradient-to-r from-[#FCD400] to-[#C59A34] bg-clip-text"> -->
            <span class="font-bold"> Pawss </span>, the computer agent that sees
            <br /> what you see and works where you work.
        </span>
        <a
            href="https://pawss.party"
            target="_blank"
            class="mt-4 rounded-full border-2 p-1 pr-4 pl-4 text-sm font-semibold"
        >
            Learn more
        </a>
    </Card>

    <Card>
        <span class="text-xl font-bold">
            For the builders. By the builders.
            <!-- We ask questions. -->
            <!-- We ask questions, we build, we break, we learn, we share. -->
        </span>
    </Card>

    <Card>
        <img src="aetheriumai.png" alt="DeepSeekret logo" class="m-4 h-24" />
        <span class="font-bold">AetheriumAI</span>
        <span class="mt-2 max-w-sm rounded-full text-sm">
            There's more to your PDFs than <br /> meets the eye. Let AI show you.
        </span>
        <a
            href="http://aetheriumai.vercel.app/?ref=cloakmind"
            target="_blank"
            class="mt-4 rounded-full border-2 p-1 pr-4 pl-4 text-sm font-semibold"
        >
            Learn more
        </a>
    </Card>

    <Card>
        <span class="max-w-md text-sm">
            We build for the love of building. Drop us an
            <a href="mailto:cloakmind@gmail.com" class="link">email</a> if we <br /> can build together, or
            talk about tech or life as builders.
        </span>
    </Card>
</div>
