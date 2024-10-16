<template>
    <div class="card" style="width: 18rem;">
    <div class="card-body">
        <h5 class="card-title">{{ usuario.nombre }} {{ usuario.apellido }}</h5>
        <p class="card-text">Edad: {{ usuario.edad }}</p>
    </div>
    </div>
</template>

<script>
export default {
    name:`Usuario`,
    props: {
    usuario: {
        type: Object,
        required: true,
        validator: function (value) {
        return (
            typeof value.nombre === 'string' &&
            typeof value.apellido === 'string' &&
            typeof value.edad === 'number'
        );
        }
    }
    }
};
</script>
<style>
                                                                                                                                                                                            </style>