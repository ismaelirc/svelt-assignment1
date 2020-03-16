<script>
    let goal = "";  
    let red = false;

    function setGoal(event){
        const val = event.target.value;
        goal = val;

        if(val.indexOf("!") >= 0){
            red = true;
        }

    }

</script>
<style>
    .h1-color{
        color: red;
    }
</style>
<div id="InputH1">
    <h1 class={red ? "h1-color": ""}>{goal}</h1>
    <input type="text" value={goal} on:input={setGoal}/>
</div>