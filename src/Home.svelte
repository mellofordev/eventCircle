<script>
    let src='https://scontent.fcok10-1.fna.fbcdn.net/v/t39.8562-6/236059786_985111022325691_1310544145856897747_n.jpg?_nc_cat=103&ccb=1-5&_nc_sid=6825c5&_nc_ohc=uoXg69lmWeMAX_eaG99&_nc_ht=scontent.fcok10-1.fna&oh=00_AT8kZ_XwIsSbp8b8UHDqNsdS01FDAZza-lO54VnzlCEJUw&oe=61C87302';
</script>
<div style="display: flex;justify-content:center;align-items:center;" >
    <img {src} alt="headerimg" class="headerimg"  />
</div>
<div class="root" style="height:auto;">
    <div class="title" >
        <h1 style="font-size: 30px; font-family:Roboto;font-weight:800px;"  >See what's happening </h1>
        <span style="font-size: 15px;" >on sctce in realtime</span>
    </div>
    <span style="padding-botton:9px;font-size: 18px; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;font-weight:800;">Top stories</span>
    <div class="topstories">
        
        <div class="card ">
            <img class="hover:scale-125" src='https://scontent.fcok10-1.fna.fbcdn.net/v/t39.8562-6/266562002_716986263038045_7764128639032761978_n.jpg?_nc_cat=106&ccb=1-5&_nc_sid=6825c5&_nc_ohc=LtxB_C7hQeYAX-s_5Ph&_nc_ht=scontent.fcok10-1.fna&oh=00_AT-MRQ2qaNSo_6zIRwTntFpseofiTB0uzEzRHsw_DcWbzw&oe=61C89944' alt='cardimg' style="border-top-left-radius: 10px;border-top-right-radius: 10px;"/>
            <div class="mintext">
            <span style="font-weight:500;margin:5px;">
				title or short discription about the blog or article 
            </span>	
        </div>
        </div>
        <div class="card ">
            <img src='https://scontent.fcok10-1.fna.fbcdn.net/v/t39.8562-6/266562002_716986263038045_7764128639032761978_n.jpg?_nc_cat=106&ccb=1-5&_nc_sid=6825c5&_nc_ohc=LtxB_C7hQeYAX-s_5Ph&_nc_ht=scontent.fcok10-1.fna&oh=00_AT-MRQ2qaNSo_6zIRwTntFpseofiTB0uzEzRHsw_DcWbzw&oe=61C89944' alt='cardimg' />
            <div class="mintext">
            <span style="font-weight:500;margin:5px;">
                title or short discription about the blog or article 
            </span>	
            </div>
        </div>
    
    </div>
</div>
<div class="billboard">
    <div style="margin:10;">
        <h2 class="bigboldtext">Title of what's happening</h2>
        <span class="mintext">A small sentence about what's the news in the college and an image on the right side.</span>
    </div>
    <img {src} alt="billimg" class="billimg" style="height:auto;width:450px;">
</div>
<div class="gallery">
    <div class="grids">
        <div class="row">
            <img {src} alt="1">
            <img {src} alt="2">
        </div>
        <div class="row">
            <img {src} alt="3" >
            <img {src} alt="4">
        </div>
    </div>
    <div class="rightgrid">
        <h1 class="bigboldtext">Title about the photo gallery</h1>
        <span class="mintext">this is a sentence where we gonna talk about the photo gallery and some news about it ,sure its dynamic and is fetch from api  </span>
    </div>
</div>
<style>
    	.card{
		display: flex;
		flex-direction: column;
		border-radius: 10px;
		box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
		height:300px;
		width:240px;
		margin:5;
		margin-right: 23px;
	}
	.card img{
		
		border-top-left-radius: 10px;
		border-top-right-radius: 10px;

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

	.gallery{
		display: flex;
		flex-direction: row;
		border-radius: 15px;
		margin: 30px;
		justify-content: space-between;
	}
	.row{
		display:flex;
		flex-direction: row;
		height:180px;
		padding:3px;
		
	}
	.row img{
		border-radius:15px;
		padding:5px;
	}
    .bigboldtext{
		font-size:25px;
		font-weight: 800;
	}
	.mintext{
		font-size:19px;
		
	}
	.topstories{
		padding:50px;
		display: flex;
		flex-direction: row;
		overflow-x: scroll;
		
	}
	.topstories ::-webkit-scrollbar{
		display:none;
	}
    .headerimg{
		width:80%;
		height:auto;
		border-radius:25px;
		padding:9px;
	}
    .title{
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;

	}
	@media (max-width: 800px) {
     .billboard {
         flex-direction: column;
		 padding: 10px;
		 margin:15px;		
       }
	   .billboard img{
		   height:auto;
		   width:100%;
		   
	   }
	   .headerimg{
		   width:500px ;
		   padding:5px;
		   border-radius: 15px;
	   }
	   .billimg{
		padding-right:0px;
		height:350px;
		border-radius: 5px;
	   }
	   
	   .gallery{
		   flex-direction: column;
		   margin:15px;
		   justify-content: center;
	   }
	   .row{
		   width:55%;
		   padding:3px;
		   

	   }
	   .topstories{
		   padding:20px;
	   }
	   .topstories::-webkit-scrollbar{
		   display: none;
	   }
	   .grids{
		overflow-x: scroll;
	   }
	   
	   .card{
		   width:350px;
	   }
    }
</style>