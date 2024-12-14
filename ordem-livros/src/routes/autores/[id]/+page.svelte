<script>
    import { page } from "$app/stores";
    import ConteudoAutor from "../../../components/autor/ConteudoAutor.svelte";
    import autores from "../../../constants/autores";
</script>

<ConteudoAutor autor={$page.data.autor} />
