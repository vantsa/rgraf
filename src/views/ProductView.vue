<template>
    <div>
        <product-header />
        <product-viewer />
        <product-garantion />
        <page-footer />
    </div>
</template>

<script>
import ProductHeader from "../components/ProductHeader.vue"
import PageFooter from "../components/PageFooter.vue"
import ProductGarantion from "../components/ProductGarantion.vue"
import ProductViewer from "../components/ProductViewer.vue"

export default {
  name: "ProductView",
  components: {
    ProductHeader,
    PageFooter,
    ProductGarantion,
    ProductViewer,
  },
}
</script>

<style scoped>
</style>
