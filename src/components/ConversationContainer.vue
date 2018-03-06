<template>
  <div>
    Conversation ID: {{id}}
    <hr>
    <Message
      v-for="message in conversation.messages"
      :message="message"
      :key="message.created"
    />
  </div>
</template>

<script>
import Message from './Message.vue'
import { mapState } from 'vuex'

export default {
  name: 'ConversationContainer',
  components: {
    Message
  },
  props: {
    conversation: {
      type: Object,
      required: true
    },
    id: {
      type: String,
      required: true
    }
  },
  created() {

  }
}
</script>

<style lang="css">
</style>
