<script>
  export let name;
</script>

<!-- use lang="sass" for SASS -->
<style lang="scss">
  $color: red;

  div {
    > p {
      background: green;
      color: white;
    }
  }

  h1 {
    color: $color;
  }
</style>

<h1>Hello {name}!</h1>

<div>
  <p>SASS is working!</p>
</div>
