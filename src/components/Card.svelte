<script lang="ts">
    export let main_content = "Basic";
    export let index = 0;
    let card_bg = "variant-glass-primary";
    index = index % 6;
    switch (index) {
        case 0:
            card_bg = "variant-glass-primary";
            break;
        case 1:
            card_bg = "variant-glass-secondary";
            break;
        case 2:
            card_bg = "variant-glass-success";
            break;
        case 3:
            card_bg = "variant-glass-danger";
            break;
        case 4:
            card_bg = "variant-glass-warning";
            break;
        case 5:
            card_bg = "variant-glass-info";
            break;
        default:
            card_bg = "variant-glass-primary";
            break;
    }
</script>

<div class="card card-hover p-4 basis-1/3 my-4 mx-12 {card_bg}">
    <header class="card-header">(header)</header>
    <section class="p-4">{main_content}</section>
    <footer class="card-footer">(footer)</footer>
    <button>red</button>
</div>
				
<style>
    .card{
        cursor: pointer;
        position: relative;
    }
    button{
        position: absolute;
        top: 0%;
        left: 100%;
        cursor: pointer;
    }
</style>
