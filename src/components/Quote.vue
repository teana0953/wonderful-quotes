<template>
    <b-col sm="6" md="4" lg="3">
        <b-card class="quote">
            <b-card-text class="quote__text">
                <slot></slot>
            </b-card-text>
        </b-card>
    </b-col>
</template>

<script></script>

<style>
.quote {
    cursor: pointer;
    margin-bottom: 20px;
}

.quote:hover {
    background-color: #ffe2e2;
}

.quote__text {
    font-family: 'Arizonia', cursive;
    font-size: 24px;
    color: #6e6e6e;
}
</style>
