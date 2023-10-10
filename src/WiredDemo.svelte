<style>
    body {
      margin: 0;
      font-family: "Gloria Hallelujah", cursive;
      font-size: 16px;
      line-height: 1.8;
    }
  
    main {
      padding: 16px;
      text-align: center;
    }
  
    wired-card {
      max-width: 400px;
      margin: 0 auto;
      padding: 20px;
      display: block;
    }
  
    section {
      max-width: 400px;
      margin: 0 auto;
      padding: 60px 0;
    }
  
    wired-button {
      background: yellow;
      color: red;
      margin: 8px;
    }
    wired-input {
      width: 200px;
      font-family: inherit;
    }
  </style>
  
  <script>
          import "wired-elements";
  
          let input;
  
          function handleClick() {
            window.alert(`Hello ${input.value.trim()}!`);
          }
  </script>
  
  <wired-card elevation="5">
    <h1>
      wired-elements demo
    </h1>
  </wired-card>
  
  <section>
    <wired-input placeholder="your name" bind:this={input}></wired-input>
    <wired-button elevation="2" on:click={handleClick}>Submit</wired-button>
  </section>