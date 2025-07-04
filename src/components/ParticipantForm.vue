<template>
  <form @submit.prevent="submitForm" class="form-container">
    <input
      type="text"
      v-model="name"
      placeholder="Masukkan nama peserta"
      class="input"
    />
    <button type="submit" class="button">Tambah</button>
    <p v-if="error" class="error">{{ error }}</p>
  </form>
</template>

<script>
export default {
  name: 'ParticipantForm',
  data() {
    return {
      name: '',
      error: ''
    }
  },
  methods: {
    submitForm() {
      if (!this.name.trim()) {
        this.error = 'Nama tidak boleh kosong!'
      } else {
        this.error = ''
        this.$emit('add-participant', this.name.trim())
        this.name = ''
      }
    }
  }
}
</script>
