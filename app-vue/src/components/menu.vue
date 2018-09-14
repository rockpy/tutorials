<template>
    <div id="menu">
        menu {{ msg }}
        <ul id="memu-ul">
            <li v-for="item in menu_list" v-bind:item="item" v-bind:key="item.id">
                {{ item.name }}
            </li>
        </ul>
    </div>
</template>

<style scoped>

#menu {
    background: #CCEBFF;
    min-height: 300px;
    padding: 16px;
}

</style>

<script>
export default {
    name: 'menu',
    props: {
        msg: String,
        menu_list: [
            {id:1, name:'Page 1', url:'page_1'},
            {id:2, name:'Page 2', url:'page_2'},
            {id:3, name:'Page 3', url:'page_3'}
        ]
    }
}
</script>
