<script>
  import Portal from '../src/Portal.svelte'
</script>

<body>
  <main>
    <div id="portalCtn">
      <Portal target="footer">
        <div id="renderedInFooter"></div>
      </Portal>
      <Portal target="#target">
        <div id="renderedInTarget"></div>
      </Portal>
      <Portal target="body > .target">
        <div id="renderedInTargetClass"></div>
      </Portal>
      <Portal
        style="position:absolute;left:50%;top:50%;transform:translate(-50%,-50%);"
      >
        <div id="renderedInDefaultWithAttributes"></div>
      </Portal>
    </div>
  </main>

  <div id="target"></div>
  <div class="target"></div>

  <footer></footer>
</body>