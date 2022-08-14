<section id="about">
	<div class="container about__container">
		<h2 class="about__title">What we <br /> do at Zibon</h2>
		<a href="/" class="contact__btn about__btn" >
			<h4>.</h4> 
		</a>

		<div class="about__left">
			<div class="about__image">
				<div class="about__image-bg" />
				<div class="about__image-lg">
					<img src="/images/aboutZibon.jpg" alt="images" />
				</div>
				<div class="about__image-sm">
					<img src="/images/aboutZibon.jpg" alt="images" />
				</div>
			</div>
		</div>

		<div class="about__right">
			<div class="empty about__empty" />
			<p>
				Zibon is a real-time location and fraud solution based application that serves as a guiding
				light to every user ensuring that your preferred products are available
			</p>
			<p>
				Zibon is a real-time location and fraud solution based application that serves as a guiding
				light to every user ensuring that your preferred products are available
			</p>
			<p>
				Zibon is a real-time location and fraud solution based application that serves as a guiding
				light to every user ensuring that your preferred products are available
			</p>
		</div> 
	</div>
</section>

<style>
	#about {
		margin-top: 18rem;
	}
	.about__container {
		display: grid;
		grid-template-columns: 10rem 26rem auto;
		/* gap:7rem; */
		position: relative;
	}
	.about__title {
		position: absolute;
		top: -13rem;
		z-index: 1;
	}

	.about__btn {
		align-self: end;
	}
	.about__image {
		position: relative;
	}
	.about__image-bg {
		width: 16rem;
		height: 24rem;
		position: absolute;
		bottom: 0;
		background: #eb9d2f;
	}
	.about__image-lg {
		position: relative;
		width: 30rem;
		left: 1rem;
		bottom: 1rem;
		filter: saturate(0) brightness(0.3);
		transition: 500ms ease;
	}
	.about__image-sm {
		position: absolute;
		top: 3rem;
		left: 8rem;
		height: 22rem;
		width: 22rem;
		overflow: hidden;
		box-shadow: 2rem 2rem 2rem rgba(0, 0, 0, 0.2);
		transition: all 400ms ease;
	}
	.about__image:hover .about__image-sm {
		opacity: 0;
	}
	.about__image:hover .about__image-lg {
		filter: saturate(1) brightness(1);
		box-shadow: 0 3rem 3rem rgba(0, 0, 0, 0.2);
		border: 0.1rem solid #eb9d2f;
	}
	.about__right {
		margin-left: 7rem;
	}
	.about__right p {
		margin: 0 0.4rem 1.5rem 0;
		font-size: 0.8rem;
	}
	.about__container h4 {
		color: black;
	}
	@media screen and (max-width: 1024px) {
		.about__container{
			grid-template-columns: 46% 54%;
			gap: 6%;

		}
		.about__image-bg, .about__image-sm {
			display: none;
		}
		.about__image-lg {
			left: 0;
			top: 0;
			filter: saturate(1) brightness(1);
			width: 100%;
			
		}
		.about__btn{
			display: none;
		}
		.about__image:hover .about__image-lg {
			border: none;
		}
		.about__right{
			margin: 0;
		}
		.about__right p {
			margin-bottom: 1rem  ;
		}
		
	}
	@media screen and (max-width: 600px) {
		.about__container{
			grid-template-columns: 1fr;
			gap: 2rem;
		}
		.about__right p {
			width: 100%;
		}
		.about__title {
			top: -7rem;
		}

	}
</style>
