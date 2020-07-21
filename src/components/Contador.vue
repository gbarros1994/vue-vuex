<template>
    <div>
        <h2 class="font-weight-light">Contador: {{contador }}</h2>
        <h4 class="font-weight-light">Contador: {{ contadorAlias }}</h4>
        <button class="btn btn-success m-2" @click="decrementar">-</button>
        <button class="btn btn-success m-2" @click="incrementar">+</button>
    </div>
</template>

<script>
import { mapState } from 'vuex'


export default {
    // computed: mapState(['contador']),
    computed: mapState({
        ...mapState({
            contador: 'contador',
            contadorAlias: 'contador'
        })
    }),
    methods: {
        decrementar() {
            this.$store.state.contador --
        },
        incrementar(){
            this.$store.state.contador ++
        }
    },
}
</script>