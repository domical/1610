<template>
    <div class="alert" :class="estadoClase">
      {{ mensaje }}
    </div>
  </template>
  
  <script>
  export default {
    name:`EstadoPedido`,
    props: {
      estado: {
        type: String,
        required: true
    }
    },
    computed: {
    mensaje() {
        switch (this.estado) {
        case 'enviado':
            return 'Tu pedido ha sido enviado.';
        case 'pendiente':
            return 'Tu pedido está pendiente.';
        case 'cancelado':
            return 'Tu pedido ha sido cancelado.';
        default:
            return 'Estado desconocido.';
        }
    },
    estadoClase() {
        if (this.estado === 'enviado') return 'alert-success';
        if (this.estado === 'pendiente') return 'alert-warning';
        if (this.estado === 'cancelado') return 'alert-danger';
        return 'alert-secondary';
    }
    }
};
</script>