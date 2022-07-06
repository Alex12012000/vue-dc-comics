<template>
    <section>
        <div class="container">
            <div class="content">
                <h3>Content goes here</h3>
            </div>
        </div>
    </section>
</template>


<script>
export default {
    name: "MainContentSection"
}
</script>

<style lang="scss" scoped>
@import "../style/common.scss";

section {
    background-color: #1c1c1c;
    .content {
        padding: 30px;
        color: white;
    }
}
</style>