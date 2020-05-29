<script>
let someText = "FullStack Software Engineer"
let count = 0

const handleClick = () => count += 1

// function handleClick(){
//     count += 1
// }

</script>

<div class="about">
    <p>{someText}</p>
    <button on:click={handleClick}>Commit</button>
    <p>Haz hecho {count} {count === 1 ? 'commit' : 'commits'}</p>
</div>

<style>
p{
    color: var(--theme-color);
    font-size: 24px;
}
</style>