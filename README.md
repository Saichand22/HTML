# HTML
Restaurant Order  taking
<!DOCTYPE html>
<html>
<head>
	<meta charset="utf-8">
	<meta name="viewport" content="width=device-width, initial-scale=1">
	<title>Royal food</title>
	<link rel="stylesheet" type="text/css" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">



	
    <link rel="stylesheet" href="https://unpkg.com/swiper/swiper-bundle.min.css"/>

</head>
<style>
	@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@100;300;400;500;700&display=swap');

:root
{
	--black: #333;
	--light-color: #c4e600;
	--box-shadow: 0 .5rem 1.5rem rgba(0,0,0,.1);
}
*
{
	font-family: 'Roboto', sans-serif;
	margin: 0;
	padding: 0;
	box-sizing: border-box;
	text-decoration: none;
	border: none;
	outline: none;
	text-transform: capitalize;
	transition: all .2s linear;
}
html
{
	font-size: 62.5%;
	overflow-x: hidden;
	scroll-behavior: smooth;
}



header
{
	position: fixed;
	top: 0;
	left: 0;
	right: 0;
	background: var(--black);
	padding: 1rem 7%;
	display: flex;
	align-items: center;
	justify-content: space-between;
	box-shadow: var(--box-shadow);
	z-index: 10000;
}
header .logo img 
{
	height: 50px;
}
header .navbar a 
{
	font-size: 1.7rem;
	padding: .5rem 1.5rem;
	color: var(--light-color);
	border: .1rem solid transparent;
}
header .navbar a.active,
header .navbar a:hover
{
	color: #fff;
	border: .1rem solid rgba(205, 170, 124, 0.2);
} 
header .icons i 
{
	cursor: pointer;
	margin-left: .5rem;
	height: 4.5rem;
	width: 4.5rem;
	line-height: 4.5rem;
	background: var(--light-color);
	text-align: center;
	font-size: 1.7rem;
	color: #fff;
}
header .icons i:hover
{
	color: #fff;
	background: var(--light-color);
	transform: rotate(360deg);
}
header .icons #menu
{
	display: none;
}








.home .home-slider .slide
{
	display: flex;
	align-items: center;
	height: 100vh;
	justify-content: flex-start;
}
.home .home-slider .slide1 
{
	background: url(https://i.pinimg.com/736x/65/89/3b/65893bf4637178a08fc41b8353defe98.jpg);
}
.home .home-slider .slide2
{
	background: url(https://img.freepik.com/premium-photo/korean-hot-spicy-chicken-flavor-ramen-instant-noodles-stir-fried-noodle_44537-725.jpg?w=2000);
}
.home .home-slider .slide3
{
	background: url(https://media.istockphoto.com/photos/grilled-chicken-legs-on-a-black-plate-picture-id1236168731?k=20&m=1236168731&s=170667a&w=0&h=GewS4cj_IAED-TaR7RLoII5XF45_T7I5dLDd22pENTg=);
}
.home .home-slider .slide1,
.home .home-slider .slide2,
.home .home-slider .slide3
{
	background-size: cover;
	background-repeat: no-repeat;
}
.home .home-slider .slide .content
{
	text-align: center;
	padding-left: 9rem;
}
.home .home-slider .slide .content h3
{
	color: var(--light-color);
	font-size: 3rem;
	font-weight: 300;
}
.home .home-slider .slide .content h1
{
	color: #fff;
	font-size: 8rem;
}
.home .home-slider .slide .content p 
{
	color: #e6e7e7;
	font-size: 1.8rem;
	letter-spacing: 1px;
	padding: .5rem 0;
	line-height: 1.5;
	font-weight: 200;
}
.btn
{
	margin-top: 1rem;
	display: inline-block;
	font-size: 1.7rem;
	color: #fff;
	border: .1rem solid rgba(205,170,124,0.2);
	background: transparent;
	cursor: pointer;
	padding: .8rem 3rem;
	position: relative;
	overflow: hidden;
	z-index: 1;
}
.btn:before
{
	content: '';
	width: 100%;
	height: 100%;
	background: var(--light-color);
	z-index: -1;
	position: absolute;
	top: 0;
	left: -100%;
	transition: .5s;
}
.btn:hover.btn:before
{
	left: 0;
}
.swiper-pagination-bullet
{
	background: var(--light-color)!important;
	width: 15px!important;
	height: 15px!important;
	border-radius: 0!important;
}










section
{
	padding: 8rem 9%;
}
.heading
{
	text-align: center;
	color: var(--black);
	font-size: 4.5rem;
	padding-bottom: 2rem;
	text-transform: uppercase;
	letter-spacing: 1.3px;
}
.sub-heading
{
	text-align: center;
	color: var(--light-color);
	font-size: 2.5rem;
	padding: .5rem 2rem;
	font-weight: 300;
	margin-bottom: 4rem;
	background: var(--black);
	display: inline-block;
}

.welcome .box-container
{
	display: flex;
	gap: 1.5rem;
}
.welcome .box-container .box
{
	width: 33%;
	background: var(--black);
	box-shadow: var(--box-shadow);
	text-align: center;
	padding-bottom: 1%;
}
.welcome .box-container .box .image
{
	height: 25rem;
	width: 100%;
	overflow: hidden;
	position: relative;
}
.welcome .box-container .box .image img 
{
	height: 100%;
	width: 100%;
	object-fit: cover;
}
.welcome .box-container .box .image:hover img 
{
	transform: scale(1.1);
}
.welcome .box-container .box .content 
{
	padding: 2rem;
	padding-top: 2rem;
}
.welcome .box-container .box .content h3
{
	color: var(--light-color);
	font-size: 2.2rem;
	font-weight: 400;
}
.welcome .box-container .box .content p 
{
	color: #fff;
	font-size: 1.4rem;
	font-weight: 300;
	padding: .5rem 0;
	line-height: 1.5;
}





 
.our-menu
{
	background: url(C:\Users\Srikanth\Downloads\pic2-removebg-preview.png) left top no-repeat, url(https://i.pinimg.com/originals/fc/0b/ca/fc0bca765c94a813eb8797590f21b2f0.jpg);

}
.our-menu .menu-container
{
	padding: 3rem 0;
	display: grid;
	grid-template-columns: repeat(auto-fit,minmax(50rem,2fr));
	gap: 5rem 10rem;
}
.our-menu .menu-container .item .item-name
{
	display: flex;
	justify-content: space-between;
	padding: 1rem 0;
	margin-top: .5rem;
}
.our-menu .menu-container .item .menu-item
{
	padding: .5rem 0;
}
.our-menu .menu-container .item .item-name h2
{
	font-size: 3rem;
	color: #e5e5e5;
	font-weight: 300;
}
.our-menu .menu-container .item .item-menu h3
{
	font-size: 2rem;
	color: #e5e5e5;
	font-weight: 200;
	display: inline-block;
}
.our-menu .menu-container .item .item-menu span 
{
	width: 37%;
	display: inline-block;
	border: 1px dotted #e5e5e5;
}
.our-menu .menu-container .item .item-menu ul 
{
	display: flex;
	font-size: 1.5rem;
	list-style: none;
	padding: .8rem 0;
	font-weight: 200;
}
.our-menu .menu-container .item .item-menu ul li a 
{
	color: #b9b9b9;
}











.our-chef
{
	width: 100%;
	display: grid;
	grid-template-columns: repeat(auto-fit,minmax(30rem,1fr));
	grid-gap: 1.5rem;
}
.our-chef .item .image img 
{
	width: 100%;
}
.our-chef .item
{
	position: relative;
	z-index: 2;
	overflow: hidden;
}
.our-chef .item:before
{
	position: absolute;
	content: '';
	width: 100%;
	height: 100%;
	display: none;
	top: 0;left: 0;right: 0;bottom: 0;
	background: rgba(0, 0, 0, .5);
	z-index: 5;
}
.our-chef .item:hover.item:before
{
	display: block;
}
.our-chef .item .chef-info
{
	position: absolute;
	top: 130%;
	left: 0;right: 0;bottom: 0;
	display: flex;
	justify-content: center;
	z-index: 10;
	align-items: center;
	transition: 1s;
	cursor: pointer;
}
.our-chef .item .chef-info h3
{
	font-size: 1.7rem;
	color: #fff;
	padding: .8rem 0;
	text-transform: uppercase;
}
.our-chef .item .chef-info span
{
	font-size: 1.7rem;
	color: var(--light-color);
	letter-spacing: 1px;
	font-weight: 300;
}
.our-chef .item .chef-info ul 
{
	list-style: none;
	display: flex;
	grid-gap: 2rem;
	padding: 3rem 0;
}
.our-chef .item .chef-info ul li a 
{
	color: #b9b6b6;
	font-size: 1.8rem;
}
.our-chef .item:hover .chef-info 
{
	top: 0;
}








.reservation
{
	display: flex;
	width: 100%;
	flex-wrap: wrap;
}
.reservation .image
{
	width: 55%;
	background: url(https://media.istockphoto.com/photos/bride-and-groom-toasting-with-red-wine-on-wedding-ceremony-picture-id479777226?k=20&m=479777226&s=612x612&w=0&h=4CPfPmrueTi2bvi8DLKrIBb01kvL7gVtRIM1_kWgfj8=);
	background-size: cover;
	background-repeat: no-repeat;
	background-position: center center;
	padding-top: 9rem;
}
.reservation .form 
{
	background: #181818;
	width: 45%;
	padding: 9rem 7%;
}
.reservation .form h1
{
	color: #fff;
}
.reservation .form-holder
{
	display: flex;
	grid-gap: 3rem;
	width: 100%;
}
.reservation .form form input,
.reservation .form form select
{
	display: block;
	margin: 2rem 0;
	width: 100%;
	background: none;
	border-bottom: .1rem solid #b7b3b3;
	color: #b7b3b3;
	font-size: 1.8rem;
	font-weight: 300;
}
.reservation .form form input:placeholder
{
	color: #b7b3b3;
}








.blog .box-container .box 
{
	background: #fff;
}
.blog .content
{
	text-align: left;
	position: relative;
}
.blog .content h3,
.blog .content p,
.blog .content a
{
	color: #333!important;
}
.blog .content a
{
	font-size: 14px;
	display: inline-block;
	padding-top: 1rem;
	text-decoration: underline;
}
.blog .content img 
{
	position: absolute;
	right: 0;
	bottom: 0;
}









.footer
{
	background: #333;
	text-align: center;
	color: #b2b2b2;
	font-size: 1.3rem;
}
.footer .container
{
	display: grid;
	grid-template-columns: repeat(auto-fit, minmax(30rem,2fr));
	color: #b2b2b2;
	grid-gap: 1rem;
	padding: 4rem 0;
	border-bottom: 1px solid #b2b2b2;
}
.footer .container div
{
	padding: 0 7rem;
}
.footer .container h3
{
	color: #fff;
	font-size: 1.5rem;
	padding-bottom: .8rem;
}
.footer .container input
{
	width: 100%;
	border: 1px solid #b2b2b2;
	padding: .5rem .8rem;
	background: transparent;
	border-radius: 20px;
}
.footer .container ul 
{
	list-style: none;
	display: flex;
	justify-content: center;
	padding-top: 1rem;
}
.footer .container ul li a 
{
	color: #b2b2b2;
	margin-left: 10px;
	font-size: 18px;
}
.footer .container span 
{
	display: block;
}











::-webkit-scrollbar{
	width: 12px;
}
::-webkit-scrollbar-track{
	background: #333;
}
::-webkit-scrollbar-thumb{
	background: #cdaa7c;
}






.topbtn
{
	position: fixed;
	right: 2%;
	bottom: 10%;
	width: 30px;
	height: 30px;
	background: #cdaa7c;
	color: #fff;
	cursor: pointer;
}








@media (max-width: 991px)
{
	html
	{
		font-size: 55%;
	}
	header
	{
		padding: 1rem 2rem;
	}
	header .logo img
	{
		height: 7rem;
	}
	.our-menu .menu-container
	{
		grid-template-columns: repeat(auto-fit,minmax(30rem,2fr));
	}
	.our-menu .menu-container .item .item-menu span 
	{
		width: 15%;
	}

}
@media (max-width: 768px)
{
	

	header .logo img
	{
		height: 7rem;
	}
	header .icons #menu
	{
		display: inline-block;
	}
	header .navbar
	{
		position: absolute;
		top: 100%;
		left: 0;
		right: 0;
		background: #eee;
		border-top: .1rem solid rgba(205,170,124,0.2);
		border-bottom: .1rem solid rgba(205,170,124,0.2);
		padding: 1rem;
		clip-path: polygon(0 0,100% 0,100% 0,0 0);
	}
	header .navbar.active
	{
		clip-path: polygon(0 0,100% 0,100% 100%,0 100%);
	}
	header .navbar a 
	{
		display: block;
		padding: 1.5rem;
		margin: 1rem;
		font-size: 2rem;
		background: var(--black);
	}

	

	.home .home-slider .slide
	{
		justify-content: center;
		height: 80vh;
	}
	.home .home-slider .slide .content
	{
		padding: 0;
	}
	.home .home-slider .slide .content h1
	{
		font-size: 7rem;
	}

	

	.welcome .box-container
	{
		flex-wrap: wrap;
	}
	.welcome .box-container .box 
	{
		width: 100%;
	}
	.reservation .image
	{
		width: 0;
	}
	.reservation .form
	{
		width: 100%;
	}
	.reservation .form .form-holder
	{
		display: block;
	}
}

   
</style>
<body>
	
	<header>
		<a href="#" class="logo"><img src="C:\Users\Srikanth\Downloads\food-logo-fork-and-knife-crown-background-vector-11381640-removebg-preview.png"></a>

		<nav class="navbar">
			<a href="#home" class="active">home</a>
			<a href="#about">about</a>
			<a href="#menu">menu</a>
			<a href="#team">team</a>
			<a href="#reservation">reservation</a>
			<a href="#blog">blog</a>
		</nav>

		<div class="icons">
			<i class="fas fa-bars" id="menu"></i>
			<i class="fas fa-search"></i>
			<i class="fas fa-heart"></i>
			<i class="fas fa-shopping-cart"></i>
		</div>





	</header>
	





	<div class="home" id="home">
		<div class="swiper home-slider">
			<div class="swiper-wrapper wrapper">
				<div class="swiper-slide slide slide1">
					<div class="content">
						<img src="C:\Users\Srikanth\Downloads\food-logo-fork-and-knife-crown-background-vector-11381640-removebg-preview.png">

						<h3>delicious royate</h3>
						<h1>gift voucher</h1>
						<p>
							give away your beloved customers
						</p>
						<a href="#" class="btn">order now</a>
					</div>
				</div>

				<div class="swiper-slide slide slide2">
					<div class="content">
						<img src="C:\Users\Srikanth\Downloads\food-logo-fork-and-knife-crown-background-vector-11381640-removebg-preview.png">

						<h3>sale of 10% this dish</h3>
						<h1>the fresh</h1>
						<p>
							food restaurant
						</p>
						<a href="#" class="btn">order now</a>
					</div>
				</div>

				<div class="swiper-slide slide slide3">
					<div class="content">
						<img src="C:\Users\Srikanth\Downloads\food-logo-fork-and-knife-crown-background-vector-11381640-removebg-preview.png">

						<h3>we are open</h3>
						<h1>fresh fruits</h1>
						<p>
							you will love it
						</p>
						<a href="#" class="btn">order now</a>
					</div>
				</div>
			</div>

			<div class="swiper-pagination"></div>
		</div>
	</div>
	
	<section class="welcome" id="about">
		<h1 class="heading">WELCOME TO ROYATE</h1>
		<center><h3 class="sub-heading"> ~ Luxury & Quality ~ </h3></center>

		<div class="box-container">
			<div class="box">
				<div class="image">
					<img src="https://media.istockphoto.com/photos/female-chef-in-kitchen-picture-id803934008?k=20&m=803934008&s=612x612&w=0&h=qyLJj6Mo-adPT2bnKCNLSD_aqBz35iLrTYE4YJhjJWk=">
				</div>

				<div class="content">
					<h3>PROFESSIONAL LEVEL</h3>
					<p>nor again is there anyone who loves or pursues or desires to obtain pain of itself, becuase it is pain, but because occasionally circumstances occur.</p>

					<a href="#" class="btn">Read More</a>
				</div>
			</div>

			<div class="box">
				<div class="image">
					<img src="https://media.istockphoto.com/photos/roasted-sea-bream-fish-with-lemon-slices-picture-id855749956?k=20&m=855749956&s=612x612&w=0&h=eycDeJxfc86J3RPfYctI1-vmQ4LyDSo_ytVXOdAmpLE=">
				</div>

				<div class="content">
					<h3>FRESH FOOD GUARANTEED</h3>
					<p>nor again is there anyone who loves or pursues or desires to obtain pain of itself, becuase it is pain, but because occasionally circumstances occur.</p>

					<a href="#" class="btn">Read More</a>
				</div>
			</div>

			<div class="box">
				<div class="image">
					<img src="https://media.istockphoto.com/photos/closeup-of-chef-throwing-sea-fruit-and-fish-picture-id1136857938?k=20&m=1136857938&s=612x612&w=0&h=fAz1hHB3krhD1JgPMurzOPZ3a5ZAb6Am7bXbfSMn6G0=">
				</div>

				<div class="content">
					<h3>THE MENU IS PLENTIFUL</h3>
					<p>nor again is there anyone who loves or pursues or desires to obtain pain of itself, becuase it is pain, but because occasionally circumstances occur.</p>

					<a href="#" class="btn">Read More</a>
				</div>
			</div>
		</div>
	</section>
	


	<section class="our-menu" id="menu">
		<h1 class="heading">our food menu</h1>
		<center><h3 class="sub-heading"> ~ see what we offer ~ </h3></center>

		<div class="menu-container">

			<div class="item">
				<div class="item-name">
					<h2>Main Course</h2>
					<img src="C:\Users\Srikanth\Downloads\icons8-cafe-100.png">
				</div>

				<div class="item-body">
					<div class="item-menu">
						<h3>Super-Delicious Zuppa Toscana</h3>
						<span class="dots"></span>
						<h3>$40</h3>

						<ul>
							<li><a href="#">Chicken</a></li>
							<li><a href="#">Italian</a></li>
							<li><a href="#">Sausage</a></li>
							<li><a href="#">Spinach</a></li>
						</ul>
					</div>

					<div class="item-menu">
						<h3>Super-Delicious Zuppa Toscana</h3>
						<span class="dots"></span>
						<h3>$26</h3>

						<ul>
							<li><a href="#">Mushrooms</a></li>
							<li><a href="#">Italian</a></li>
							<li><a href="#">Sausage</a></li>
							<li><a href="#">Spinach</a></li>
						</ul>
					</div>

				</div>
			</div>

			<div class="item">
				<div class="item-name">
					<h2>Soups & salads</h2>
					<img src="C:\Users\Srikanth\Downloads\icons8-cafe-100.png">
				</div>

				<div class="item-body">
					<div class="item-menu">
						<h3>Super-Delicious Zuppa Toscana</h3>
						<span class="dots"></span>
						<h3>$40</h3>

						<ul>
							<li><a href="#">Chicken</a></li>
							<li><a href="#">Italian</a></li>
							<li><a href="#">Sausage</a></li>
							<li><a href="#">Spinach</a></li>
						</ul>
					</div>

					<div class="item-menu">
						<h3>Super-Delicious Zuppa Toscana</h3>
						<span class="dots"></span>
						<h3>$26</h3>

						<ul>
							<li><a href="#">Mushrooms</a></li>
							<li><a href="#">Italian</a></li>
							<li><a href="#">Sausage</a></li>
							<li><a href="#">Spinach</a></li>
						</ul>
					</div>

				</div>
			</div>


			<div class="item">
				<div class="item-name">
					<h2>Drinks</h2>
					<img src="C:\Users\Srikanth\Downloads\icons8-cafe-100.png">
				</div>

				<div class="item-body">
					<div class="item-menu">
						<h3>Super-Delicious Zuppa Toscana</h3>
						<span class="dots"></span>
						<h3>$40</h3>

						<ul>
							<li><a href="#">Chicken</a></li>
							<li><a href="#">Italian</a></li>
							<li><a href="#">Sausage</a></li>
							<li><a href="#">Spinach</a></li>
						</ul>
					</div>

					<div class="item-menu">
						<h3>Super-Delicious Zuppa Toscana</h3>
						<span class="dots"></span>
						<h3>$26</h3>

						<ul>
							<li><a href="#">Mushrooms</a></li>
							<li><a href="#">Italian</a></li>
							<li><a href="#">Sausage</a></li>
							<li><a href="#">Spinach</a></li>
						</ul>
					</div>

				</div>
			</div>


			<div class="item">
				<div class="item-name">
					<h2>Desserts</h2>
					<img src="C:\Users\Srikanth\Downloads\icons8-cafe-100.png">
				</div>

				<div class="item-body">
					<div class="item-menu">
						<h3>Super-Delicious Zuppa Toscana</h3>
						<span class="dots"></span>
						<h3>$40</h3>

						<ul>
							<li><a href="#">Chicken</a></li>
							<li><a href="#">Italian</a></li>
							<li><a href="#">Sausage</a></li>
							<li><a href="#">Spinach</a></li>
						</ul>
					</div>

					<div class="item-menu">
						<h3>Super-Delicious Zuppa Toscana</h3>
						<span class="dots"></span>
						<h3>$26</h3>

						<ul>
							<li><a href="#">Mushrooms</a></li>
							<li><a href="#">Italian</a></li>
							<li><a href="#">Sausage</a></li>
							<li><a href="#">Spinach</a></li>
						</ul>
					</div>

				</div>
			</div>

		</div>
	</section>
	


	<section class="our-team" id="team">
		<h1 class="heading">our talented chef</h1>
		<center>
			<h3 class="sub-heading"> ~ Experience $ Enthusiasm ~ </h3>
		</center>

		<div class="our-chef">
			<div class="item">
				<div class="image">
					<img src="https://images.unsplash.com/photo-1581299894007-aaa50297cf16?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=387&q=80">
				</div>

				<div class="chef-info">
					<div>
						<h3>Jerry robertson</h3>
						<span>master chef</span>

						<ul>
							<li><a href="#"><i class="fa-brands fa-instagram"></i></a></li>
							<li><a href="#"><i class="fa-brands fa-twitter"></i></a></li>
							<li><a href="#"><i class="fa-brands fa-whatsapp"></i></a></li>
							<li><a href="#"><i class="fa-brands fa-linkedin-in"></i></a></li>
						</ul>
					</div>
				</div>
			</div>

			<div class="item">
				<div class="image">
					<img src="https://images.unsplash.com/photo-1574966740793-953ad374e8fe?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1yZWxhdGVkfDF8fHxlbnwwfHx8fA%3D%3D&auto=format&fit=crop&w=500&q=60">
				</div>

				<div class="chef-info">
					<div>
						<h3>Corol rowson</h3>
						<span>master chef</span>

						<ul>
							<li><a href="#"><i class="fa-brands fa-instagram"></i></a></li>
							<li><a href="#"><i class="fa-brands fa-twitter"></i></a></li>
							<li><a href="#"><i class="fa-brands fa-whatsapp"></i></a></li>
							<li><a href="#"><i class="fa-brands fa-linkedin-in"></i></a></li>
						</ul>
					</div>
				</div>
			</div>

			<div class="item">
				<div class="image">
					<img src="https://images.unsplash.com/photo-1577219491135-ce391730fb2c?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1yZWxhdGVkfDEzfHx8ZW58MHx8fHw%3D&auto=format&fit=crop&w=500&q=60">
				</div>

				<div class="chef-info">
					<div>
						<h3>taylor mccoy</h3>
						<span>master chef</span>

						<ul>
							<li><a href="#"><i class="fa-brands fa-instagram"></i></a></li>
							<li><a href="#"><i class="fa-brands fa-twitter"></i></a></li>
							<li><a href="#"><i class="fa-brands fa-whatsapp"></i></a></li>
							<li><a href="#"><i class="fa-brands fa-linkedin-in"></i></a></li>
						</ul>
					</div>
				</div>
			</div>


		</div>
	</section>
	


	
		<div class="reservation" id="reservation">
			<div class="image">
				
			</div>

			<div class="form">
				<h1 class="heading">book a table</h1>
				<center><h3 class="sub-heading">~ check out our place ~ </h3></center>

				<form>
					<div class="form-holder">
						<div>
							<select>
								<option>1 people</option>
								<option>2 people</option>
								<option>3 people</option>
								<option>4 people</option>
							</select>

							<input type="text" name="" placeholder="Time">
							<input type="text" name="" placeholder="Phone">
						</div>

						<div>
							<input type="text" name="" placeholder="Date">
							<input type="text" name="" placeholder="Name">
							<input type="email" name="" placeholder="email">
						</div>
					</div>
					<center><a href="#" class="btn">Book now</a></center>
				</form>
			</div>
		</div>
	


	<section class="blog welcome" id="blog">
		<h1 class="heading">latest news</h1>
		<center><h3 class="sub-heading"> ~ Greate articles ~ </h3></center>

		<div class="box-container">
			<div class="box">
				<div class="image">
					<img src="https://media.istockphoto.com/photos/closeup-of-table-setting-for-hanukkah-family-meal-picture-id1343862553?k=20&m=1343862553&s=612x612&w=0&h=G0j0pIjGEvTWTS3RJxvCifRe4dL7QzQ86tm04f23ra8=">
				</div>

				<div class="content">
					<h3>PROFESSIONAL LEVEL</h3>
					<p>nor again is there anyone who loves or pursues or desires to obtain pain of itself, becuase it is pain, but because occasionally circumstances occur.</p>
					<a href="#">READ MORE</a>
			
				</div>
			</div>

			<div class="box">
				<div class="image">
					<img src="https://media.istockphoto.com/photos/indian-dal-food-traditional-indian-soup-lentils-indian-dhal-spicy-in-picture-id1130228947?k=20&m=1130228947&s=612x612&w=0&h=z1budiElUOKjJS2jzj5exddTycSXZ_oseU7kzOuZI24=">
				</div>

				<div class="content">
					<h3>FRESH FOOD GUARANTEED</h3>
					<p>nor again is there anyone who loves or pursues or desires to obtain pain of itself, becuase it is pain, but because occasionally circumstances occur.</p>
					<a href="#">READ MORE</a>
					
				</div>
			</div>

			<div class="box">
				<div class="image">
					<img src="https://media.istockphoto.com/photos/glass-of-red-wine-and-wine-bottles-on-the-background-picture-id856530520?k=20&m=856530520&s=612x612&w=0&h=NohMqO7QkCHs4MwQOWEbnT813rD3S5PlvjmbRllqsIA=">
				</div>

				<div class="content">
					<h3>THE MENU IS PLENTIFUL</h3>
					<p>nor again is there anyone who loves or pursues or desires to obtain pain of itself, becuase it is pain, but because occasionally circumstances occur.</p>
					<a href="#">READ MORE</a>
					
				</div>
			</div>

		</div>
	</section>
	
	

	
	<section class="footer">
		<img src="C:\Users\Srikanth\Downloads\food-logo-fork-and-knife-crown-background-vector-11381640-removebg-preview.png" class="logo">

		<div class="container">
			<div>
				<h3>ABOUT US</h3>
				<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod.</p>
			</div>

			<div>
				<h3>GET NEWS & OFFERS</h3>
				<input type="email" name="" placeholder="enter your email">
				<ul>
					<li><a href="#"><i class="fa-brands fa-twitter"></i></a></li>
					<li><a href="#"><i class="fa-brands fa-instagram"></i></a></li>
					<li><a href="#"><i class="fa-brands fa-whatsapp"></i></a></li>
					<li><a href="#"><i class="fa-brands fa-linkedin-in"></i></a></li>
				</ul>
			</div>

			<div>
				<h3>CONTACT US</h3>
				<span>Dharshan</span>
				<span>+ (91) 1234567890</span>
				
				
			</div>
		</div>

		
	</section>
	<a href="#"><button class="topbtn"><i class="fa-solid fa-angle-up"></i></button></a>

	
    <script src="https://unpkg.com/swiper/swiper-bundle.min.js"></script>

    
    <script>
      var swiper = new Swiper(".home-slider", {
        spaceBetween: 30,
        centeredSlides: true,
        autoplay: {
          delay: 7500,
          disableOnInteraction: false,
        },
        pagination: {
          el: ".swiper-pagination",
          clickable: true,
        },
        loop:true,
      });
    </script>
	<script type="text/javascript">
		let menu = document.querySelector('#menu');
		let navbar = document.querySelector('.navbar');

		menu.onclick = () =>{
			menu.classList.toggle('fa-times');
			navbar.classList.toggle('active');
		}
	</script>
</body>
</html>
