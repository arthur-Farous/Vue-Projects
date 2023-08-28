<script setup>


</script>

<template>
    <div class="design">
     <nav>
        <slot name="first_nav"></slot>
     </nav>
     <section>
        <slot name="mobile"></slot>
     </section>
     <footer>
        <slot name="desktop"></slot>
     </footer>

    </div>

</template>


<style scoped>
.design{
    display: flex;
    flex-flow: column;
    justify-content: center;
    align-items: center;
    gap:10px
}

.desktop,.mobile{
    background-color: blue;
    color: black;
}
</style>