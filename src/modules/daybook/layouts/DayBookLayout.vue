<template>
    <NavbarComp />

    <div class="d-flex">
        <div class="col-4">
            <EntryList />
        </div>
        <div class="col">
            <RouterView />
        </div>
    </div>
</template>

<script>

import { defineAsyncComponent } from "vue";

export default {
    components: {
        NavbarComp: defineAsyncComponent(() => import('@/modules/daybook/components/NavbarComp.vue')),
        EntryList: defineAsyncComponent(() => import('@/modules/daybook/components/EntryList.vue'))
    }
}
</script>