<template>
    <v-container>
        <Crud v-if="store.user != null"/> 
    <div v-else>
        não logado
    </div>
    </v-container>
</template>
<script setup>
import { useAuthStore } from '@/store/AuthLogon';
import Crud from '@/components/Crud.vue';

const store = useAuthStore();
</script>