<script>
  export let style
</script>

<h1 style={style}>
  <slot />
</h1>

<style lang="scss" scoped>
  @import "../../styles/_variables.scss";
  h1 {
    font-size: 1.7rem;
    color: #171717;
    letter-spacing: 1px;
    font-weight: 800;
    margin-bottom: 2rem;
    margin-top: 0px;
    text-align: center;
  }

  // colors
  h1 {
    color: $dark-text-primary;
  }
</style>
