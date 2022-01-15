<script>
    
    import {createClient} from '@supabase/supabase-js';
    const supabaseUrl = __api.env.SVELTE_APP_SUPABASE_URL
    const supabaseAnonKey = __api.env.SVELTE_APP_SUPABASE_ANON_KEY

    let src ='https://assets.awwwards.com/awards/images/2019/05/illustration-web-design-2-cover.jpg'
    const supabase = createClient(supabaseUrl,supabaseAnonKey)
    const login =async ()=>{
		const {user,session,error} = await supabase.auth.signIn({
		provider:'google',
	})
    console.log(user);
    
	}
</script>
<svelte:head>
    <title>login</title>
</svelte:head>
<main>
    <img {src} alt="loginimg" class="loginimg" />
    
    <div class="logincard">
        <img {src} alt="loginimg" class="loginimgdesktop"/>
        <h1>Register your free account</h1>
        <button class="loginbtn" on:click={login}>Login with google</button>
    </div>

</main>
<style>
    main{
        height: 600px;
        
    }
    h1{
        font-size: 20px;
        font-family: Roboto;
        font-weight: 800;
        text-align: center;
    }
    .loginimg{
        width: 100%;
        display:none;      
    }
    .loginimgdesktop{
        width:100%;
        display:block;
        border-top-right-radius:15px;
        border-top-left-radius: 15px;
    }
    .logincard{
        display:flex;
        flex-direction: column;
        background-color: rgb(32, 32, 32);
        margin: 23px;
        border-radius: 15px;
        padding-bottom: 6px;
        width:50%;
        justify-content: center;
    }
    .loginbtn{
        background-color: white;
        border-radius: 15px;
        width: auto;
        border-color: black;
        font-size: 25px;
        margin:5px;
        color:black;
    }
    .loginbtn:hover{
        background-color: whitesmoke;
        border-color: black;
    }
     @media(max-width:800px){
         .loginimg{
             display: block;
         }
         .logincard{
            width:auto;
         }
         .loginimgdesktop{
             display:none;
         }
     }
</style>