<template>
    <div>
        <b-card :title="name"
                style="max-width: 20rem;"
                class="mb-2">
            <p class="card-text">
                Some quick example text to build on the card title and make up the bulk of the card's content.
            </p>
            <b-button :href="url" variant="primary">Open</b-button>
            <div slot="footer">
                <b-badge variant="secondary" class="system-tag" v-for="tag in tags">{{tag}}</b-badge>
            </div>
        </b-card>
    </div>
</template>

<script>
    export default {
        name: 'SystemInfo',
        props: {
            name: String,
            tags: Array,
            url: String
        }
    };
</script>

<style scoped>
    .card-text {
        font-family: monospace;
    }
    .system-tag {
        padding: inherit 1rem;
    }
</style>