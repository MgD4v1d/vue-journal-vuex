<template>
    <div class="entry-container pointer p-3"
        @click="$router.push({name: 'entry', params: {id: 10}})"
    >
        <!-- titulo -->
        <div class="entry-title d-flex">
            <span class="text-success fs-5 fw-bold">18</span>
            <span class="mx-1 fs-5">Enero</span>
            <span class="mx-2 fw-light">2022, Martes</span>
        </div>

        <div class="entry-description">
            Lorem ipsum dolor sit, amet consectetur adipisicing elit. Blanditiis quidem recusandae laborum, sint eligendi assumenda, ullam eos cumque dicta nam delectus obcaecati. Sequi aut tempora provident neque voluptatum at deleniti!
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>

.entry-container{
    border-bottom: 1px solid #2c3e50;
    transition: 0.2s all ease-in;

    &:hover{
        background-color: lighten($color: gray, $amount: 45);
        transition: 0.2s all ease-in;
    }

    .entry-description{
        font-size: 12px;
    }
}

</style>