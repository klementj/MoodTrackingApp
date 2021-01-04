<template>
  <h2>Hvordan har du det?</h2>
  <form id="test">
    <EmojisRating />
    <TextInput label="Title" placeholder="Klarede opvasken 💪"/>
    <TextArea label="Beskrivelse" placeholder="Kunne ikke overskue at vaske op hele sidste uge. Havde et kæmpe bjerg og gemte mig mest under dynen. I dag havde jeg bare ekstra energi. Måske var det fordi jeg fik snakket med Niels om vores aftale i næste uge."/>
    <SubmitButton label="Gem minde"/>
  </form>
</template>

<script>
import TextInput from '../atoms/textInput.vue'
import TextArea from '../atoms/textArea.vue'
import EmojisRating from './emojisRating.vue'
import SubmitButton from '../atoms/submitButton.vue'
  
export default {
  name: 'AddForm',

  components: {
    TextInput,
    TextArea,
    EmojisRating,
    SubmitButton
  }
}
</script>

<style scoped>
form {
  @apply flex flex-col;
}
</style>
