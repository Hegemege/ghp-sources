<template>
    <div class="nav-container flex-container-vertical flex-justify-end">
        <div class="flex-container centered">
            <div class="nav-row flex-container flex-item flex-space-around">
                <div>
                    <a>Lorem Ipsum</a>
                </div>

                <div>
                    <a class="nav-link">RIGHT</a>
                    <a class="nav-link">RIGHT2</a>
                    <a class="nav-link">RIGHT3</a>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import { Component, Vue } from "vue-property-decorator";

@Component({})
export default class Nav extends Vue {}
</script>

<style lang="scss">
@import "@/style.scss";

.nav-container {
    background-color: $common-background-color-dark;

    @media (min-width: $mobile) {
        min-height: 7em;
    }

    .nav-row {
        padding: 1em;

        .nav-link {
            padding-left: 0.5em;
            padding-right: 0.5em;
        }
    }
}
</style>