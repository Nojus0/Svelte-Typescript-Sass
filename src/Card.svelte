<script lang="ts">
  export let Header: string;
  export let Description: string;
  export let ButtonText: string;
</script>

<div>
  <h1>{Header}</h1>
  <p>{Description}</p>
  <button>{ButtonText}</button>
</div>

<style lang="scss">
  div {
    h1 {
      margin: 1rem;
    }
    p {
      flex-grow: 1;
      margin: 1.2rem;
      word-wrap: break-word;
      font-size: 1.1rem;
    }
    button {
      align-self: flex-end;
      margin: 1rem;
      border: none;
      -webkit-user-select: none;
      -moz-user-select: none;
      border-radius: 0.3rem;
      cursor: pointer;
      background: rgb(226, 226, 226);
      box-shadow: 5px 5px 5px rgba(0, 0, 0, 0.24);
      transition: background 250ms ease, transform 50ms ease;
      &:hover {
        color: #fff;
        background: rgb(65, 65, 65);
      }
      &:active {
        transform: scale(1.02);
      }
    }

    display: flex;
    flex-direction: column;
    width: 20rem;
    height: 20rem;
    background: rgba(0, 0, 0, 0.062);
    border-radius: 0.25rem;
    box-shadow: 5px 5px 8px rgba(0, 0, 0, 0.281);
  }
</style>
