<template>
    <div class="entry-title d-flex justify-content-between p-2">
        <div>
            <span class="text-success fs-3 fw-bold">15</span>
            <span class="mx-1 fs-3">Julio</span>
            <span class="mx-2 fs-4 fw-light">2022, Jueves</span>
        </div>
        <div>
            <button class="btn btn-danger">
                Borrar
                <i class="fa fa-trash-alt"></i>
            </button>

            <button class="btn btn-primary">
                Subir foto
                <i class="fa fa-upload"></i>
            </button>
        </div>
    </div>
    
    <hr>

    <div class="d-flex flex-column px-3 h-75">
        <textarea 
            placeholder="¿Que sucedio hoy?"></textarea>
    </div>

    <FabComp icon="fa-light fa-floppy-disk" />

    <img
        src="https://concepto.de/wp-content/uploads/2015/03/paisaje-e1549600034372.jpg"
        alt="Entry Picture"
        class="img-thumbnail">

</template>

<script>
import { defineAsyncComponent } from 'vue';

export default {
    components: {
        FabComp: defineAsyncComponent(() => import('@/modules/daybook/components/FabCom.vue'))
    }
}
</script>

<style lang="scss" scoped>
    textarea {
        font-size: 20px;
        height: 100%;
        border: none;

        &:focus {
            outline: none;
        }
    }

    img {
        width: 200px;
        position: fixed;
        bottom: 150px;
        right: 20px;
        box-shadow: 0px 5px 10px rgba($color: #000000, $alpha: 0.5);
    }
</style>