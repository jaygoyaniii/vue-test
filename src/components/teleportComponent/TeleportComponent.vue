<template>
    <h3>Teleport Component</h3>
    <teleport to="#footer">
        <FooterTeleport />
    </teleport>
</template>

<script>
    import FooterTeleport from './FooterTeleport.vue';
    export default {
        name: "TeleportComponent",
        components: {
            FooterTeleport
        }
    }
</script>