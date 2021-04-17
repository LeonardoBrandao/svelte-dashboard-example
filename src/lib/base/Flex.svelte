<div class="flex-div">
  <slot />
</div>

<style lang="scss">
  .flex-div {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
  }
</style>
