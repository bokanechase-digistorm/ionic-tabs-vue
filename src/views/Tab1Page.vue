<template>
    <ion-page>
        <ion-header>
            <ion-toolbar>
                <ion-title>Tab 1</ion-title>
            </ion-toolbar>
        </ion-header>
        <ion-content :fullscreen="true">
            <ion-button router-link="/tabs/tab1/view1">Go To Inner View 1</ion-button>
            <ion-button router-link="/tabs/tab1/view1">Go To Inner View 2</ion-button>
            <p>Steps to replicate bug:</p>
            <ul>
                <li>Open Tab 1 - Inner View 1</li>
                <li>Switch to Tab 2</li>
                <li>Switch back to Tab 1 (should still be on Inner View 1)</li>
                <li>Replace with Tab 1 - Inner View 2</li>
                <li>Try pressing the back button or switching to Tab 2, neither work</li>
            </ul>
        </ion-content>
    </ion-page>
</template>

<script setup lang="ts">
    import {IonPage, IonHeader, IonToolbar, IonTitle, IonContent, IonButton} from '@ionic/vue';
</script>
