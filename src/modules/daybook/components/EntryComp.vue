<template>
    <div 
        class="entry-container mb-3 pointer p-2"
        @click="$router.push({name: 'entry', params: {id:10}})">
        <!-- TITULO -->
        <div class="entry-title d-flex align-items-baseline">
            <span class="text-success fs-5 fw-bold">15</span>
            <span class="mx-1 fs-5">Julio</span>
            <span class="mx-2 fw-light">2021, Jueves</span>
        </div>
        <div class="entry-description">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Maxime repellat beatae, perferendis pariatur laboriosam quasi expedita dolores voluptatum reprehenderit dolore reiciendis tempora tenetur provident nisi quo accusamus facilis. Vitae, velit!
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.entry-container {
    border-bottom: 1px solid #2c3e50;
    transition: 0.2s all ease-in;

    &:hover {
        background-color: lighten($color: rgb(83, 81, 81), $amount: 45);
        transition: 0.2s all ease-in;
    }

    .entry-description {
        font-size: 12px;;
    }
}
</style>