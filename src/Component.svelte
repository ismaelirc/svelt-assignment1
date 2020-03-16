<script>
    
    let goal = "";  
    
    $: shouldRed = goal.includes('!');

</script>
<style>
    .h-color{
        color: red;
    }
</style>
<div id="InputH1">
    <h1 class:h-color={shouldRed}>{goal}</h1>
    <input type="text" bind:value={goal} />
</div>