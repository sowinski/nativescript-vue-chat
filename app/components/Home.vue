<template>
    <Page>
        <ActionBar>
            <Label text="Home"/>
        </ActionBar>

        <DockLayout>
            <StackLayout dock="bottom">
                <DockLayout stretchLastChild="true" class="msg-box">
                    <Button text="Send" dock="right" />
                    <TextView editable="true" text="Sample message">
                    </TextView>
                </DockLayout>
            </StackLayout>
            <ScrollView dock="top">
                <StackLayout class="home-panel">
                    <!--Add your page content here-->
                    <Label textWrap="true" text="Play with NativeScript!"
                        class="h2 description-label" />
                    <Label textWrap="true"
                        text="Write code in the editor or drag and drop components to build a NativeScript mobile application."
                        class="h2 description-label" />
                    <Label textWrap="true"
                        text="Scan the QR code with your mobile device and watch the changes sync live while you play with the code."
                        class="h2 description-label" />
                    <Label textWrap="true"
                        text="Scan the QR code with your mobile device and watch the changes sync live while you play with the code."
                        class="h2 description-label" />
                </StackLayout>
            </ScrollView>
        </DockLayout>
    </Page>
</template>

<script>
  export default {
    computed: {
      message() {
        return "Blank {N}-Vue app";
      }
    }
  };
</script>

<style scoped lang="scss">
    @import '@nativescript/theme/scss/variables/blue';

    // Custom styles
    .fas {
        @include colorize($color: accent);
    }

    .info {
        font-size: 20;
        horizontal-align: center;
        vertical-align: center;
    }

    .msg-box {
        background-color: red;
    }
</style>
