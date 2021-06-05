<template>
  <footer id="main-site-footer">
    <p>
      <small>Copyright &copy;2021 Agape Connection.</small>
    </p>
    <address>
      Built by <a href="http://www.tomrembrown.com">Tom Brown</a>
    </address>
  </footer>
</template>

<script>
export default {
  name: 'Footer',
}
</script>

<style lang="scss">
#main-site-footer {
  grid-area: footer;
  display: flex;
  justify-content: space-between;

  a {
    text-decoration: none;
  }

  address {
    font-style: normal;
  }

  small {
    font-size: 0.875rem;
  }

  p {
    margin: 0;
    display: inline;
  }
}
</style>
