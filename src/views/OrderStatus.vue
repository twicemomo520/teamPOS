<script>
import LeftBar from '@/components/LeftBar.vue'
import OrderStatusComponent from '@/components/orderStatus/OrderStatusComponent.vue';
export default {
    data() {
        return {

        }
    },
    components: {
        LeftBar,
        OrderStatusComponent
    },
}
</script>

<template>
    <div class="big">
        <div class="leftBar">
            <LeftBar />
        </div>
        <div class="mainArea">
            <OrderStatusComponent />
        </div>
    </div>
</template>

<style scoped lang="scss">
.big {
    width: 100%;
    height: 100dvh;
    display: flex;
    justify-content: center;
    align-items: center;

    .leftBar {
        width: 10%;
        height: 96.4vh;
        position: fixed;
        top: 2%;
        left: 1.4%;
        display: flex;
        align-items: center;
    }


    .mainArea {
        width: 100%;
        height: 100%;
        overflow-y: scroll;
        scrollbar-width: none;
        display: flex;
        justify-content: start;
        align-items: center;
        flex-direction: column;
    }
}
</style>