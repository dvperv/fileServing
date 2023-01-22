<script>
    import {ListGroupItem} from "sveltestrap";
    export let name =" ", url = ""
</script>

<ListGroupItem>
    <a href={url} download>Загрузить {name}</a>
</ListGroupItem>