<template>
    <footer>
        <div class="block">
            <ul>
                <li><router-link to="/">Home</router-link></li>
            </ul>
            <ul>
                <li><router-link to="/about">About</router-link></li>
            </ul>
            <ul>
                <li><router-link to="/contact">Contact</router-link></li>
            </ul>
        </div>
    </footer>
</template>

<script>
export default {
    name: "footer"
}
</script>

<style lang="scss" scoped>
    footer {
        width: 100%;
        background-color: #005cb2;
        color: white;
        height: 40vh;
        margin-top: 5%;
        padding-top: 2%;
    }
    .block {
        display: grid;
        width: 90%;
        height: 100%;
        grid-template-columns: 1fr 1fr 1fr;
        grid-template-rows: 1fr 1fr 1fr;
        margin: 0 5%;
        & li {
            list-style-type: none;
        }
        & a:hover, a {
            all: unset;
            color: white;
            cursor: pointer;
        }
    }
</style>