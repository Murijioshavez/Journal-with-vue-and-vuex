<template>
    <div class="entry-tittle d-flex justify-content-between p-2">
        <div>
            <span class="text-center fs-3 fw-bold">15</span>
            <span class="mx-1 fs-3 ">julio</span>
            <span class="mx-2 fs-4 fw-light">2023, jueves</span>
        </div>
        <div>
            <button class="btn btn-danger mx-2">
                Borrar
                <i class=" fa fa-trash-alt"></i>
            </button>

            <button class="btn btn-primary">
                subir foto
                <i class=" fa fa-upload"></i>
            </button>
        </div>
    </div>
    <hr>
    <div class="d-flex flex-column px-3 h-75">
        <textarea placeholder="¿Qué sucedió hoy?"></textarea>
    </div>
    <Fav 
        icon="fa-save"
    />
    <img src="https://i.pinimg.com/236x/05/cf/5b/05cf5bd4bdad7cb94797a886d787c945.jpg" 
    alt="entry-picture"
    class="img-thumbnail">
</template>


<script>
import { defineAsyncComponent } from 'vue'
export default {
    components: {
        Fav: defineAsyncComponent(()=> import('../components/Fav.vue'))
    }
}
</script>

<style lang="scss" scoped>

textarea{
    font-size: 20px;
    border: none;
    height: 100%;

    &:focus {
        outline: none;
    }
}
img{
    width: 200px;
    position: fixed;
    bottom: 150px;
    right: 20px;
    box-shadow: 0px  5px 10px rgba($color: #000000, $alpha: 0.2)
}

</style>