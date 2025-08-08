<template>
    <ion-page>
        <ion-header>
            <ion-toolbar>
                <ion-buttons slot="start">
                    <ion-back-button/>
                </ion-buttons>
                <ion-title>Tab 1 - Inner View 2</ion-title>
            </ion-toolbar>
        </ion-header>

        <ion-content fullscreen color="light">
            <p>Tab 1 - Inner View 2</p>

            <ion-button @click="ionRouter.replace('/tabs/tab1/view1')">Replace With Inner View 1</ion-button>
        </ion-content>
    </ion-page>
</template>

<script setup lang="ts">
    import {IonPage, IonHeader, IonToolbar, IonButtons, IonBackButton, IonTitle, IonContent, useIonRouter} from '@ionic/vue';
    const ionRouter = useIonRouter();
</script>

<style scoped>

</style>