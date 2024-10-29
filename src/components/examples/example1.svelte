<script>
    let count = 1;
    $: double = count * 2;
    console.log(double);
</script>

<button on:click={() => {
    count++;
    console.log(count, double);
}}>count: {count}, double: {double}</button>