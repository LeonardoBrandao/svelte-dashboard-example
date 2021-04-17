<div class="spacing">
  <div class="card">
    <slot />
  </div>
</div>

<style lang="scss">
  @import "../../styles/_variables.scss";
  .spacing {
    padding: 10px;
    flex-grow: 1;
  }
  .card {
    background: #fff;
    box-shadow: 2px 4px 20px 4px rgba(0, 0, 0, 0.15);
    border-radius: 10px;
    padding: 15px 20px;
  }

  // colors
  .card {
    background: $dark-bg-tertiary;
  }
</style>
