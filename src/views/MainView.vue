<template>
    <div>
        <page-header />
        <first-content />
        <second-content />
        <garantion-comp />
        <third-content />
        <fourth-content />
        <fifth-content />
        <sixth-content />
        <garantion-comp />
        <page-footer />
    </div>
</template>

<script>
import PageHeader from '../components/PageHeader.vue'
import FirstContent from '../components/FirstContent.vue'
import SecondContent from '../components/SecondContent.vue'
import GarantionComp from '../components/GarantionComp.vue'
import ThirdContent from '../components/ThirdContent.vue'
import FourthContent from '../components/FourthContent.vue'
import FifthContent from '../components/FifthContent.vue'
import SixthContent from '../components/SixthContent.vue'
import PageFooter from '../components/PageFooter.vue'

export default {
  name: "MainView",
  components: {
    PageHeader,
    FirstContent,
    SecondContent,
    GarantionComp,
    ThirdContent,
    FourthContent,
    FifthContent,
    SixthContent,
    PageFooter,
  },
}
</script>

<style scoped>
</style>
