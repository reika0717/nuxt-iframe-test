<template>
  <section class="container">
    <div>
      <iframe src="http://penqe.com/iframe_test.html" frameborder="0" id="filecontainer"></iframe>
    </div>
  </section>
</template>

<script>
import $ from "jquery";

export default {
  mounted() {
    var iframe = $("#filecontainer").contents();

    iframe.find("#target").click(function() {
      console.log("CLICKED");
    });
  }
};
</script>

<style>
</style>
