<script>
  export let type
</script>

<button on:click class="{`base-button base-button-${type ? type : 'default'}`}"><slot /></button>

<style lang="scss">
  @import "../../styles/_variables.scss";
  .base-button {
  border: none;
  border-radius: 100px;
  padding: 8px 25px;
  font-weight: 700;
  background: #fff;
  font-size: 1rem;
  cursor: pointer;
  font-family: $font-family;
  border: 2px solid transparent;
  transition: all $transition-speed ease-in-out;
  min-width: 115px;

  // smooth text animation
  backface-visibility: hidden;
  transform: translateZ(0);
  -webkit-font-smoothing: subpixel-antialiased;

  &-default {
    color: #2d2d2d;
    background-color: #f7f7f7;
    &:hover,
    &:focus {
      border-color: #7b7b7b;
    }
  }
  &-danger {
    color: #fff2f2;
    background-color: #ff6767;
    &:hover,
    &:focus {
      border-color: #800;
    }
  }
  &-primary {
    color: #2d2d2d;
    background-color: #00b8ff;
    &:hover,
    &:focus {
      border-color: rgb(0, 132, 255);
    }
  }
  &-alert {
    color: #2d2d2d;
    background-color: #ffae00;
    &:hover,
    &:focus {
      border-color: #b96f00;
    }
  }
  &-success {
    color: #2d2d2d;
    background-color: #9dff00;
    &:hover,
    &:focus {
      border-color: #008c00;
    }
  }
  &-dark {
    color: #ffffff;
    background-color: #1d1e22;
    &:hover,
    &:focus {
      border-color: #a5a5a5;
    }
  }
}

</style>
