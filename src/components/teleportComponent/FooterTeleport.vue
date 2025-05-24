<template>
    <div class="footer">
        <h3>Footer Teleport</h3>
        <p>Copyright @Code Step By Step</p> 
    </div>
</template>

<script>
    export default {
        name: "FooterTeleport"
    }
</script>

<style>
.footer{
    background-color: #333;
    color: white;
    padding: 10px;
    display: flex;
    justify-content: center;
    align-items: center;
    position: fixed;
    bottom: 0;
    width: 100%;
}
</style>