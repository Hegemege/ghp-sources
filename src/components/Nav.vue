<template>
    <div class="nav-container flex-container-vertical flex-justify-end">
        <div class="flex-container centered">
            <div class="nav-row flex-container flex-item flex-space-around">
                <div>
                    <a>Lorem Ipsum</a>
                </div>

                <div>
                    <a class="ext-icon" href="https://github.com/Hegemege" target="_blank"><font-awesome-icon :icon="['fab', 'github']" /></a>
                    <a class="ext-icon" href="https://www.linkedin.com/in/henriniva/" target="_blank"><font-awesome-icon :icon="['fab', 'linkedin']" /></a>
                    <a class="ext-icon" href="https://twitter.com/Hegemege" target="_blank"><font-awesome-icon :icon="['fab', 'twitter']" /></a>
                    <div class="nav-separator"></div>
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

        .nav-separator {
            display: inline-block;
            min-width: 2em;
        }

        .ext-icon {
            margin-left: 0.5em;
            text-decoration: none;

            &:visited {
                color: $common-text-color;
            }

            cursor: pointer;
        }

        .nav-link {
            padding-left: 1em;
        }
    }
}
</style>