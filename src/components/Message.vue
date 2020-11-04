<template>
  <div>
    <img :src="message.sender.profileImage" alt="Profile pic" title="Profile pic" >
    <p :id="[!message.read ? 'read' : '']" >
      <span id="nom">{{message.sender.name}}</span> <br/>
      <span >{{message.date}}</span> <br/>
      <span > {{message.content}} </span>
    </p> <br/>
  </div>
</template>

<script>
export default {
  name: "Message",
  props:{
    message: Object,
  }
}
</script>

<style scoped>
#nom {
  font-weight: bold;
}
#read {
  color:  blue;

}
h1 {
  border: solid red 2px;
}
</style>
