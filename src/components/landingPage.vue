<template>
  <div class="content">
      <about-me
        v-if="!showCurriculum"
        @openCurriculum="showCurriculum = true"
      />
      <curriculum
        v-else
        @close="showCurriculum = false"
      />
  </div>
</template>

<script>
import AboutMe from '../components/aboutMe'
import Curriculum from '../components/curriculum'

export default {
  components: {
    AboutMe,
    Curriculum
  },
  data() {
    return {
      showCurriculum: false
    }
  },
}
</script>

<style scoped lang="scss">
  .content {
    position: absolute;
    background-color: rgba(0, 0, 0, .6);
    padding: 30px;
    border-radius: 10px;
    z-index: 30;

    @media only screen and (max-width: 768px) {
      width: 100%;
      height: 100%;
    }

    
  }
</style>
