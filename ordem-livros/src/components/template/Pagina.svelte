<script>
    import AreaLateral from "./AreaLateral.svelte";
    import Cabecalho from "./Cabecalho.svelte";
    import Rodape from "./Rodape.svelte";
</script>

<div
    class="
     flex flex-col
    bg-black text-white min-h-screen
    "
>
    <Cabecalho />
    <div class="flex-1 flex gap-5 max-w-7xl mx-auto w-full p-5">
        <main class="flex-1">
            <slot></slot>
        </main>
        <AreaLateral />
    </div>
    <Rodape />
</div>
