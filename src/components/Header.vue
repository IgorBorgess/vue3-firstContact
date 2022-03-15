<template>
    <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">Projetos</a></li>
        <li><a href="#">Contato</a></li>
        <li v-if="logged_in"><a href="#">My profile</a></li>
    </ul>
</template>

<script>
export default {
    name: "Header",
    props: ["logged_in"]
}
</script>

<style scoped>
    ul {
        list-style: none;
        display: flex;
        background-color: #999;
    }

    li {
        margin-right: 10px;
    }

    a {
        color: #DDD;
        text-decoration: none;
        transition: .5s;
    }

    a:hover {
        color: turquoise;
    }
</style>