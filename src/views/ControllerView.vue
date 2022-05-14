<template>
    <div>
        <div class="title">
            <h1>맘잡고 카페 키오스크</h1> <br>
            <h3>맘잡고 카페에 오신 것을 환영해요.</h3>
        </div>

        <br>
        <button @click="increase">증가</button>
        <button @click="decrease" style="margin-left: 10px;">감소</button>
        <br><br>
        <button @click="icetea">아이스티 4100원</button> &nbsp;&nbsp;
        <button @click="icetea_cl">아이스티 취소</button> <br>
        <button @click="ameri">아메리카노 4600원</button> &nbsp;&nbsp;
        <button @click="ameri_cl">아메리카노 취소</button> <br>
        <button @click="latte">카페라떼 5300원</button> &nbsp;&nbsp;
        <button @click="latte_cl">카페라떼 취소</button> <br>
        <button @click="mocha">카페모카 5500원</button> &nbsp;&nbsp;
        <button @click="mocha_cl">카페모카 취소</button> <br>
        <button @click="cancel">전체 취소</button>
        <br><br>
        <h3>키오스크</h3>
    </div>
</template>

<script>

    export default {
        methods : {
            increase() {
                this.$store.state.count++;
            },
            decrease() {
                this.$store.state.count--;
            },
            icetea() {
                this.$store.state.count += 4100;
            },
            icetea_cl() {
                this.$store.state.count -= 4100;
            },
            ameri() {
                this.$store.state.count += 4600;
            },
            ameri_cl() {
                this.$store.state.count -= 4600;
            },
            latte() {
                this.$store.state.count += 5300;
            },
            latte_cl() {
                this.$store.state.count -= 5300;
            },
            mocha() {
                this.$store.state.count += 5500;
            },
            mocha_cl() {
                this.$store.state.count -= 5500;
            },
            cancel() {
                this.$store.state.count = 0;
            },
        }
    }
</script>

<style lang="stylus" scoped>
</style>