<script lang="ts">
    export let serie: any = null;
</script>

{#if serie}
    <a
        href="/series/{serie.id}"
        class="flex flex-col rounded-md overflow-hidden border-zinc-800 border"
    >
        <img
            src={serie.imagem}
            alt="Imagem da Série"
            class="h-96 object-cover"
        />
        <div class="flex flex-col gap-2 p-5">
            <span class="text-2xl font-black">{serie.titulo}</span>
            <span class="text-sm text-zinc-400 text-justify"
                >{serie.descricao}</span
            >
            <button class="botao azul font-semibold self-end">Leia mais</button>
        </div>
    </a>
{/if}
