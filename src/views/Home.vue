<template>
  <div class="home">
    <Main />
    <Chat />
  </div>
</template>

<script>
import Main from '../components/Main';
import Chat from '../components/Chat';


export default {
  name: 'Home',
  components: {
    Main,
    Chat
  }
}
</script>
