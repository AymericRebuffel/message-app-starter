
<template>
  <div id="tout">
    <h1>Ceci est Messages</h1>
    <div>
      <Message v-for="currentMessage in messages" :key="currentMessage.id" :message="currentMessage"></Message>
    </div>
  </div>
</template>

<script>
import {messagesMock} from '@/mocks/messages.mock';
import Message from "@/components/Message";
export default {
  name: "Messages",
  components: { Message},
  data(){
    return {
      messages: messagesMock
    };
  }
}

</script>

<style scoped>

#tout {
  border: solid blue 2px;
}
</style>
