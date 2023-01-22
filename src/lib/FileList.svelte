<script>
    import {ListGroup} from "sveltestrap";
    import FileListItem from "./FileListItem.svelte";
    let files = [
        { id: 1, url: "http://localhost:8085/more_static/1" },
        { id: 2, url: "http://localhost:8085/more_static/2" },
        { id: 3, url: "http://localhost:8085/more_static/3" },
    ]
</script>

<ListGroup>
    {#each files as file}
        <FileListItem name={file.id} url = {file.url} />
    {/each}
</ListGroup>