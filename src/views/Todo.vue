<template>

  <div>
    
    <MO @Input="validate"></MO>
    <KO :K1="K1"></KO>
    </div>
    
</template>

<script>
import MO from "../components/MO.vue"
import KO from "../components/KO.vue"
export default {
  data: () => ({
    K1: [],
  }),
components :{MO,KO},
K1: "Input",
  methods: {
    validate(select, name) {
      this.K1.push({
        name: select + " : " + name,
      });
    },
  },
};
</script>

<style>

</style>