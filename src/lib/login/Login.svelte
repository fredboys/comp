<script>
    export let showModal
    export let loggedIn


    function toggle() {
		loggedIn = !loggedIn;
	}
</script>

<div class="signin"> 
    <div class="content"> 
     <h2>LOGIN & PLAY</h2> 
     <div class="form">
        <p>Login with your prefered method</p>
        <button on:click={toggle} class="btn">Google</button>
        <button on:click={toggle} class="btn">Facebook</button>
        <button on:click={toggle} class="btn">Microsoft</button>
      <button on:click={() => (showModal = true)} class="btn rules"> Rules </button>
     </div> 
    </div> 
   </div>
   
<style>
    @font-face {
        font-family: 'Gelasio';
        font-style: normal;
        font-weight: 400;
        src: local('Gelasio Regular'), local('Gelasio-Regular'), url(https://fonts.gstatic.com/s/gelasio/v1/cIf9MaFfvUQxTTqS9C6hYQ.woff2) format('woff2');
        unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
    }
    .signin
{
  position: absolute;
  width: 400px;
  background: #222;  
  z-index: 1000;
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 40px;
  border-radius: 4px;
  box-shadow: 0 15px 35px rgba(0,0,0,9);
}
.signin .content 
{
  position: relative;
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  gap: 5px;
}
.signin .content h2 
{
  font-size: 2em;
  color: #0f0;
  text-transform: uppercase;
  margin-bottom: 5px;
  font-family: 'Gelasio';
}
.signin .content .form 
{
  width: 100%;
  display: flex;
  flex-direction: column;
  gap: 25px;
  text-align: center;
}
p {
    color: #0f0;
    font-weight: 400;
    font-size: 20px;
    font-family: 'Gelasio';
}

.btn {
    background: #0f0;
    color: #000;
    font-family: 'Gelasio';
    font-weight: 600;
    font-size: 1.35em;
    letter-spacing: 0.05em;
    cursor: pointer;
    padding: 10px;
    border-radius: 4px;
    border: none;
    outline: none;    
}

.btn:hover{
  letter-spacing: 3px;
  font-size: 1.5em;
  background: #fff;
  color: #000;
}
.rules {
    margin-top: 15px;
}
</style>