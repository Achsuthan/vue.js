<template>
<div>
    <p> Current status : {{status}}</p>
    <hr/>
    <button @click="changeStatusFn()">Change Status</button>
</div>
</template>
<script>
export default {
    data(){
        return {
            status: "Normal"
        }
    },
    methods: {
        changeStatusFn: function() {
            console.log(this.status)
            this.status = "Critical" 
        }
    },
}
</script>