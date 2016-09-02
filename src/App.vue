<template>
  <div id="app">
    <Navbar></Navbar>
<!--     <Billet></Billet>
    <Foot></Foot> -->
    <add></add>
  </div>
</template>

<script>
import Billet from './components/Billet'
import Navbar from './components/Navbar'
import Foot from './components/Foot'
import add from './components/AjouterBillet'

export default {
  components: {
    Foot,
  	Navbar,
    Billet,
    add
  }
}
</script>

<style>
</style>
