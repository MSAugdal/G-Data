<template>
    <div>
        <h1>This is a graph of you steps. lorem ipsum</h1>
        <img src="../assets/graph.png" alt="amazing graph">
    </div>
</template>

<style scoped>
@import '../assets/base.css';
h1 {
    font-size: 3rem;
    font-weight: 400;
}
img {
    max-width: 100%;
    border-radius: 8px;
    border: 2px solid var(--accent-400);
}
div {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    gap: 2rem;
}
</style>
