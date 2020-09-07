<template>
<div>
    <a v-if="!color" class="navbar-brand" href="#"><img src="@/assets/logo.png" alt="picture"></a>
    <a v-if="color" class="navbar-brand" href="#"><img src="@/assets/LogoWhite.png" alt="picture"></a>
</div>

</template>

<script>
export default {
    props: ['color']
}
</script>

<style>

</style>