<template>
    <b-row>
        <form>
            <b-col sm="8" offset-sm="2" xs="12" md="6" offset-md="3" class="form-group">
                <label>Quote</label>
                <textarea class="form-control" rows="3" v-model="quote"></textarea>
            </b-col>
            <b-col sm="8" offset-sm="2" xs="12" md="6" offset-md="3" class="form-group">
                <button class="btn btn-primary" @click.prevent="createNew">Add Quote</button>
            </b-col>
        </form>
    </b-row>
</template>

<script>
export default {
    data: function() {
        return {
            quote: '',
        };
    },
    methods: {
        createNew() {
            this.$emit('quoteAdded', this.quote);
            this.quote = '';
        },
    },
};
</script>

<style scoped>
form {
    width: 100%;
}
</style>
