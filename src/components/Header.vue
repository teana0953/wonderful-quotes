<template>
    <b-row class="header">
        <b-col col sm="12">
            <h3 class="header__title">Quotes Added</h3>
            <b-progress class="header_progress" :max="maxQuotes">
                <b-progress-bar :value="quoteCount">
                    <span>{{ quoteCount }} / {{ maxQuotes }}</span>
                </b-progress-bar>
            </b-progress>
        </b-col>
    </b-row>
</template>

<script>
export default {
    props: ['quoteCount', 'maxQuotes'],
};
</script>

<style scoped>
.header__title {
    margin-top: 20px;
}
.header_progress {
    height: 20px;
    margin-bottom: 20px;
}
</style>
