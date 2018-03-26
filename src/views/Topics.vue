<template>
    <div class="sign-in">
        <header>
            <h1>Galvanize Votes</h1>

        </header>
        <main>
        <p>This is a topic wrapper</p>
        <router-view></router-view>
        </main>
    </div>
</template>

<script>
// @ is an alias to /src
//    import HelloWorld from "@/components/HelloWorld.vue"
export default {
    name: "Topics",
    components: {
    }
}
</script>

<style scoped lang="scss">
    @import "~@/styles/_colors";
    @import "~@/styles/_typography";
    .topics {
        @include base-font;
        header {
            padding: 1rem;
            background-color: $dark-color;
            color: $white;
            @include-primary-header-font
            h1 {
                @include primary-header-font;
                text-align: center;
            }
            img {
                max-width: 320px;
                margin-bottom: 2rem;
            }
        }
        main {
            p {
                text-align: center;
            }
        }
    }
</style>
