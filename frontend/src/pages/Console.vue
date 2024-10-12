<template>
    <transition name="slide-fade" appear>
        <div>
            <h1 class="mb-3">Console</h1>

            <Terminal class="terminal" :rows="20" mode="mainTerminal" name="console" :endpoint="endpoint"></Terminal>
        </div>
    </transition>
</template>

<script>

export default {
    components: {
    },
    data() { },
    computed: {
        endpoint() {
            return this.$route.params.endpoint || "";
        },
    },
    mounted() {

    },
    methods: {

    }
};
</script>

<style scoped lang="scss">
.terminal {
    height: 410px;
}
</style>
