<template>
  <div class="item1-view-container">
    <Box title="The QuickBooks Calculator">
      <QuickBooksCalculator/>
      <SocialMediaIcons />
    </Box> 
    <FrequentlyAskedQuestions />
  </div>
</template>

<script>
import Box from '@/components/Box.vue'
import FrequentlyAskedQuestions from '@/components/FrequentlyAskedQuestions.vue'
import QuickBooksCalculator from '@/components/QuickBooksCalculator.vue'
import SocialMediaIcons from '@/components/SocialMediaIcons.vue'
export default {
  name: 'Home',
  components: { 
    Box, 
    FrequentlyAskedQuestions,
    QuickBooksCalculator,
    SocialMediaIcons
  }
}
</script>

<style scoped>
  .item1-view-container{
    display: grid;
    justify-content: center;
    align-content: center;
  }

</style>
