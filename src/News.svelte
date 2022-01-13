<script>
    let src='https://static.vecteezy.com/system/resources/previews/002/207/823/non_2x/retro-neon-lights-abstract-background-free-vector.jpg'
</script>
<svelte:head>
    <title>news</title>
</svelte:head>
<main>
    <img {src} class="newshimg" alt="newsheaderimg"  />
    <h1 style="margin-left:5px;">news</h1>
    <div class="billboard">
        <div style="margin:10;">
            <h2 class="bigboldtext" style="font-size:20px;">Title of what's happening</h2>
            <span class="mintext">A small sentence about what's the news in the college and an image on the right side.</span>
        </div>
        <img {src} alt="billimg" class="billimg" style="height:auto;width:450px;">
    </div>
</main>



<style>
    main{
        height: auto;
    }
    h1{
        font-size: 45px;
        font-family: Roboto;
        font-weight:800;
    }
    .newshimg{
        display: none;
    }
    .billboard{
		display:flex;
		flex-direction: row;
		justify-content:space-evenly;
		background-color:rgb(32,32,32);
		height:auto;
		padding:10px;
		margin:30px;
		border-radius:10px;
	}
	.billimg{
		padding-right:60px;
	}
    @media(max-width:800px){
        .newshimg{
            display:block;
            width: 100%;
        }
        .billboard {
         flex-direction: column;
		 padding: 10px;
		 margin:15px;		
       }
	   .billboard img{
		   height:auto;
		   width:100%;
		   
	   }
       .billimg{
		padding-right:0px;
		height:350px;
		border-radius: 5px;
	   }
    }

</style>