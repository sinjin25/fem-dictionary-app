<template>
    <div class="d-flex jc-sb">
        <IconLogo class="top-logo"></IconLogo>
        <div class="top-right d-flex ai-c">
            <div class="top-font-select">Mono</div>
            <IconArrowDown class="top-arrow-down"></IconArrowDown>
            <div class="top-border"></div>
            <div class="top-switch d-flex">
                <div class="top-switch-spacer-l"></div>
                <div class="top-switch-knob"></div>
                <div class="top-switch-spacer-r"></div>
            </div>
            <IconMoon class="top-moon"></IconMoon>
        </div>
    </div>
</template>

<script lang="ts" setup>
import IconLogo from './icon/Logo.vue'
import IconArrowDown from './icon/ArrowDown.vue'
import IconMoon from './icon/Moon.vue'
</script>

<style lang="scss" scoped>
.top {
    &-right {
        gap: 16px;
    }

    &-logo {
        width: 28px; //28x32
        height: 32px;
    }

    &-font-select {
        color: var(--b-3);
    }

    &-arrow-down {
        width: 12px;
        height: 8px;
    }

    &-border {
        width: 1px;
        height: 100%;
        background: var(--gray-2);
    }

    &-switch {
        padding: 3px;
        min-width: 40px;
        border-radius: 10px;

        background: var(--gray-1);

        &-knob {
            width: 14px;
            height: 14px;
            border-radius: 50px;
            background: var(--white);
        }

        &-spacer {
            &-l {
                flex: 0 0 1px;
            }

            &-r {
                flex: 0 0 1px;
            }
        }
    }

    &-moon {
        width: 20px;
        height: 20px;
        margin-left: -4px; // designs wants 12px between this and prev element for some reason
        // this needs to be able to change color
        stroke: var(--gray-1);
    }
}

.--dark .top {
    &-font-select {
        color: var(--white);
    }

    &-switch {
        background: var(--gray-1);

        &-knob {
            background: var(--white);
        }
    }
}
</style>