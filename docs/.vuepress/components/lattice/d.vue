<template>
    <div class="c-item">
        <c-row gutter="10" justify="start">
            <c-col span="6"><div class="c-block"></div></c-col>
            <c-col span="6"><div class="c-block"></div></c-col>
            <c-col span="6"><div class="c-block"></div></c-col>
        </c-row>
        <c-row gutter="10" justify="end">
            <c-col span="6"><div class="c-block"></div></c-col>
            <c-col span="6"><div class="c-block"></div></c-col>
            <c-col span="6"><div class="c-block"></div></c-col>
        </c-row>
        <c-row gutter="10" justify="center">
            <c-col span="6"><div class="c-block"></div></c-col>
            <c-col span="6"><div class="c-block"></div></c-col>
            <c-col span="6"><div class="c-block"></div></c-col>
        </c-row>
        <c-row gutter="10" justify="space-between">
            <c-col span="6"><div class="c-block"></div></c-col>
            <c-col span="6"><div class="c-block"></div></c-col>
            <c-col span="6"><div class="c-block"></div></c-col>
        </c-row>
        <c-row gutter="10" justify="space-around">
            <c-col span="6"><div class="c-block"></div></c-col>
            <c-col span="6"><div class="c-block"></div></c-col>
            <c-col span="6"><div class="c-block"></div></c-col>
        </c-row>
    </div>
</template>

<script>
import Col from '../../../../src/lattice/col'
import Row from '../../../../src/lattice/row'
export default {
    components: {
        'c-col': Col,
        'c-row': Row
    }
}
</script>

<style lang="scss" scoped>
.c-item * {
    box-sizing: border-box;
}
.row {
    margin: 10px 0;
}
.c-block {
    min-height: 30px;
    background-color: #e5e9f2;
    border-radius: 3px;
}
.col:nth-child(2n) .c-block{
    background-color: #d3dce6;
}
.row:last-child {
    margin-bottom: 0;
}
.row:first-child {
    margin-top: 0;
}
.c-item {
    border: 1px solid #d1d5da;
    padding: 24px 24px;
    margin: 1em 0;
}
</style>