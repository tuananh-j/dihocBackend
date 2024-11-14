<template>
    <p>
        cuốn sách của tôi {{ message() }}
    </p>
    <p>
        số này {{ num }} là số {{ num % 2 == 0 ? 'chẵn' : 'không chẵn' }}
    </p>
</template>

<script>
export default {
    data() {
        return {
            num: 15
        };
    },
    methods: { // Sửa từ 'method' thành 'methods'
        message() {
            return 'tôi là peto';
        }
    }
};
</script>

<style>
</style>
