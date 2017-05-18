//home.vue
<template>
    <div>
        <ol>
            <li v-for="todo in todos">
                {{todo.text}}
            </li>
        </ol>
        <button @click="eClick">click</button>
    </div>
</template>
<script>
    export default {
        name:'indexP',
        data(){
            return {
                todos:[
                    { text: 'Learn JavaScript' },
                    { text: 'Learn Vue' },
                    { text: 'Build something awesome' }
                ]
            }
        },
        methods:{
            eClick(){
                console.log(999);
            }
        }
    }
</script>