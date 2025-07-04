<template>
  <div class="app-container">
    <h1 class="title">Arisan New Era</h1>
    <ParticipantForm @add-participant="addParticipant" />
    <ParticipantList :participants="participants" @remove="removeParticipant" />
  </div>
</template>

<script>
import ParticipantForm from './components/ParticipantForm.vue'
import ParticipantList from './components/ParticipantList.vue'

export default {
  name: 'App',
  components: {
    ParticipantForm,
    ParticipantList
  },
  data() {
    return {
      participants: []
    }
  },
  methods: {
    addParticipant(name) {
      if (!this.participants.includes(name)) {
        this.participants.push(name)
      }
    },
    removeParticipant(index) {
      this.participants.splice(index, 1)
    }
  }
}
</script>
