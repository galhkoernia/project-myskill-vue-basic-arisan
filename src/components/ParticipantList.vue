<template>
  <div>
    <h2 class="list-title">Daftar Peserta</h2>
    <transition-group name="fade" tag="ul" class="participant-list">
      <li v-for="(name, index) in participants" :key="name" class="participant-item">
        {{ name }}
        <button @click="$emit('remove', index)" class="remove-btn">x</button>
      </li>
    </transition-group>
  </div>
</template>

<script>
export default {
  name: 'ParticipantList',
  props: ['participants']
}
</script>
