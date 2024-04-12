<template>
    <div class="wrapper">
        <form @submit.stop.prevent="$router.push('/dataviz')">
            <h1>GåData Login</h1>
            <div>
                <label for="navn">Fornavn og etternavn</label>
                <input name="navn" type="text" placeholder="Fornavn og etternavn">
            </div>

            <div>
                <label for="epost">E-Post</label>
                <input name="epost" type="text" placeholder="E-Post">
            </div>

            <div>
                <label for="passord">Passord</label>
                <input name="passord" type="password" placeholder="Passord">
            </div>

            <input type="submit" value="Submit">
        </form>
    </div>
</template>

<style scoped>
@import '../assets/base.css';
.wrapper{
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}
h1 {
    color: var(--text-800);
}

form {
    display: grid;
    grid-column: 1fr;
    grid-row: 1fr 1fr 1fr 1fr;

    row-gap: 1rem;

    background-color: hsla(0, 100%, 100%, 90%);
    border-radius: 8px;
    padding: 1rem 4rem 4rem 4rem;
}

div {
    display: flex;
    flex-direction: column;
}
input {
    padding: .5rem 1rem;
    border-radius: 8px;
    border: 1px solid black;
}
input[type="submit"] {
    transition: .5s;
    background-color: var(--primary-400);
    color: white;
    font-weight: 500;
    border: none;
/*    border: 2px solid var(--primary-700)*/
}
input[type="submit"]:hover {
    transition: .25s;
    box-shadow: 2px 4px var(--primary-600);
    transform: scale(1.02);
}
</style>
