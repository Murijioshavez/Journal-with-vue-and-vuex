<template >
    <div class="entry-container mb-3 pointer p-2"
    @click="$router.push({name: 'entry', params: {id: 10}})">

        <div class="entry-tittle d-flex">
            <span class="text-success fs-5 fw-bold">15</span>
            <span class="mx-1 fs-5">julio</span>
            <span class="mx-2 fw-light">2023, jueves</span>
        </div>
        <div class="entry-description">
            Fugiat laborum fugiat ex anim occaecat aute. Deserunt commodo velit eu in aliquip magna dolore tempor. Cillum elit do reprehenderit ipsum. Sit pariatur aliquip eiusmod voluptate ipsum enim adipisicing cillum ullamco.
        </div>

    </div>
</template>

<script>

</script>

<style lang="scss" scoped>
.entry-container{
    border-bottom: 1px solid #2c3e50;
    transition: 0.2s all ease-in;

    &:hover{
        background-color: lighten($color: grey, $amount: 45) ;
    }

    .entry-description{
        font-size: 12px;
    }

}
</style>