<template v-for="book in books">
    <div>
        <h1>{{ title }}</h1>
        <ul>
            <li>{{ book.title }},{{ book.author }}</li>
        </ul>
    </div>
</template>

<script>
export default {
    name: BookList,
    data () {
        books:[
            {title: 'Self-Reliance', author: 'Ralph Waldo Emerson'},
            {title: 'American Gods', author: 'Neil Gaiman'},
            {title: 'Amusing Ourselves to Death', author: 'Neil Postman'},
        ]
        return {
            title: "All Books"
        }
    }
}
</script>

<style scoped>
    h1, h2 {
        font-weight: normal;
    }
    ul{
        list-style-type: none;
        padding: 0;
    }
    li{
        display: block;
        margin: 0 10px;
    }

</style>
