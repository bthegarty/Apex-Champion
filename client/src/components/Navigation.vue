<template>
    <section class="navbar">
        <ul>
            <li><a href="/">Apex</a></li>
            <li><a href="/pubg">PUBG</a></li>
        </ul>
    </section>
</template>

<script>
export default {
    name: 'Navigation'
}
</script>

<style scoped>
    .navbar {
        background: rgba(0, 0, 0, 0.6);
        display: flex;
        justify-content: center;
        left: 0;
        position: absolute;
        top: 0;
        width: 100%;
    }

    ul {
        display: flex;
        padding: 0;
        list-style: none;
    }

    li {
        margin: 10px 15px;
    }
</style>