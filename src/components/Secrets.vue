<template>
    <div>
        THIS PAGE IS NOT USED!
    </div>
</template>

<script>
    export default {
        name: `secrets`,
        data(){
            return{
                secretString : ["What is this?", "Did you find this?", "You must be a treasure hunter"]
            }
        },
        methods: {
            showSecret(){
                const mySecret = document.querySelector(`div`);
                for (let string of this.secretString){
                    mySecret.insertAdjacentHTML(`beforeend`, `<p>>${string}</p>`)
                }
            },
            stringColor(event){
                let target = event.target;
                target.style.color = `pink`;
            }
        },
        mounted(){
            this.showSecret();
            document.querySelector(`p`).addEventListener(`click`, this.stringColor);
        },
    }
</script>

<style scoped>

</style>