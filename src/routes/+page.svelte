<script>
	import Modal from '$lib/Modal.svelte';
    import Login from '$lib/login/Login.svelte';
    import Play from '$lib/play/Play.svelte';

	let showModal = true;
    let loggedIn = false;

</script>

<Modal bind:showModal>
	<h1 slot="header" class="welcome">
		Welcome to "GAME NAME"
	</h1>
    <div class="rules">
    <h3>RULES:</h3>
	<ul class="definition-list">
		<li>You pay £1 to enter</li>
		<li>You have a time limit to achieve the highest score you can</li>
		<li>Depending on where you place, you will earn money</li>
		<li>1st - 25% of entry pot</li>
        <li>2nd - 15% of entry pot</li>
        <li>3rd - 10% of entry pot</li>
        <li>4th-10th - 1% each of entry pot</li>
		<li class="underline">EXAMPLE</li>
		<li>100,000 players</li>
        <li>1st - £25,000</li>
        <li>2nd - £15,000</li>
        <li>3rd - £10,000</li>
        <li>4th-10th - £1000 each</li>
        <li>You many enter again once your time limit runs out</li>
        <li>Competition opens every Sunday 9am and closes 9pm</li>
        <li> The more people who play, the more money you can make, so go get your <strong>FRIENDS, FAMILY</strong> and <strong>DOG</strong> online</li>
	</ul>
</div>
</Modal>

 <body> <!-- partial:index.partial.html --> 

  <section> 
    <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> 
    <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> 
    <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> 
    <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> 
    <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> 
    <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> 
    <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> 
    <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> 
    <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> 
    <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> 
    <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> 
    <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> 
    <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> 
    <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> 
    <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> 
    <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> 
    <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> 
    <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> 
    <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> 
    <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> 
    <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> 
    <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> 
    <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> 
    <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> 
    <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> 
    <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> 
    <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> 
    <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> 
    <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> 
    <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> 
    <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> 
    <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> 
    <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> 
    <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> <span></span> 
    
    {#if loggedIn }
    <Play bind:showModal/>
    {:else}
    <Login bind:loggedIn bind:showModal />
    {/if}
  </section> <!-- partial --> 
 </body>




<style>
    .rules, .welcome {
        text-align: center;
    }
    ul {
        list-style-type: none;
        padding-left: 0;
    }
    li {
        margin-bottom: 10px;
    }
    .underline {
        text-decoration: underline;
    }
    h3 {
        margin: 5px;
    }
   
*
{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
body 
{
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 100vh;
  background: #000;
}
section 
{
  position: absolute;
  width: 100vw;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 2px;
  flex-wrap: wrap;
  overflow: hidden;
}
section::before 
{
  content: '';
  position: absolute;
  width: 100%;
  height: 100%;
  background: linear-gradient(#000,#0f0,#000);
  animation: animate 5s linear infinite;
}
@keyframes animate 
{
  0%
  {
    transform: translateY(-100%);
  }
  100%
  {
    transform: translateY(100%);
  }
}
section span 
{
  position: relative;
  display: block;
  width: calc(6.25vw - 2px);
  height: calc(6.25vw - 2px);
  background: #181818;
  z-index: 2;
  transition: 1.5s;
}
section span:hover 
{
  background: #0f0;
  transition: 0s;
}
@media (max-width: 900px)
{
  section span 
  {
    width: calc(10vw - 2px);
    height: calc(10vw - 2px);
  }
}
@media (max-width: 600px)
{
  section span 
  {
    width: calc(20vw - 2px);
    height: calc(20vw - 2px);
  }
}

</style>