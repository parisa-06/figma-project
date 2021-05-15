<template >
  <div class="app">
     <Header />
   <Dashboard />
  </div>
  
</template>

<script>
import Header from "./components/Header";
import Dashboard from "./components/Dashboard";


export default {
  components: {Header,Dashboard}
}
</script>