<template>
<div>
    <template v-for ="server in 5">
        <server-status :key="server"></server-status>
    </template>
    
</div>
</template>
<script>
import ServerStatus from '../Components/ServerStatus'
export default {
    components:{
        'server-status': ServerStatus
    }
}
</script>