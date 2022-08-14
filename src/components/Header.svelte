<header>
	<div class="container header_container">
		<div class="header__left">
			<div class="header__image-bg" />
			<div class="header__image-lg">
				<img src="/images/zibonHero.jpg" alt="header_image" />
			</div>
			<div class="header__image-sm">
				<img src="/images/zibonHero.jpg" alt="header_image" />
			</div>
		</div>
		<div class="header__right">
			<div class="header__head">
				<div class="empty header__empty" />
				<a href="/" class="header__tag">#Fast Rising startUp</a>
			</div>
			<h1>Secured Products Right Next To You in RealTime</h1>
			<p>
				Lorem ipsum dolor sit amet, consectetur adipisicing elit. Eaque nulla itaque delectus illum
				cum. Et sequi nobis hic harum facilis.
			</p>
			<a href="mailto:sarmuelypmd@gmail.com" class="header__btn-md">Request Demo</a>
		</div>
	</div>
</header>
<div class="header__frames">
	<div class="header__frame">
		<img src="/images/zibonFrameA.jpg" alt="frame_images" />
	</div>
	<div class="header__frame">
		<img src="/images/zibonFrameB.jpg" alt="frame_images" />
	</div>
</div>

<style>
	header {
		height: 100vh;
		max-width: 100vw;
		position: relative;
		top: 0;
		background: linear-gradient(to right, #141e30, #243b55);
		overflow: hidden;
	}
	.header_container {
		display: grid;
		grid-template-columns: 43% 53%;
		gap: 4%;
		margin-top: 9rem;
		position: relative;
	}
	.header__image-bg {
		background-color: #eb9d2f;
		height: 22rem;
		width: 16rem;
		position: absolute;
	}
	.header__image-lg {
		width: 29rem;
		position: relative;
		top: 1rem;
		left: 1rem;
		filter: saturate(0) brightness(0.3);
		transition: all 400ms ease;
	}
	.header__image-sm {
		width: 28rem;
		height: 28rem;
		overflow: hidden;
		position: absolute;
		left: 6rem;
		top: 6rem;
		transition: all 400ms ease;
	}
	.header__left:hover .header__image-sm {
		opacity: 0;
	}
	.header__left:hover .header__image-lg {
		filter: saturate(1) brightness(1);
		/* border: .5rem solid #EB9D2F; */
		top: 0;
		left: 0;
	}
	.header__head {
		display: flex;
		gap: 2rem;
	}
	.empty {
		height: 3.5rem;
		width: 18rem;
		background-color: #141e30;
		border-radius: calc(3.5rem / 2);
		margin-bottom: 3.5rem;
		box-shadow: inset 0 1rem 1rem rgba(0, 0, 0, 0.7);
		border: 1px solid #243b55;
	}
	.header__tag {
		color: #eb9d2f;
	}
	.header__right p {
		margin-top: 2rem;
		width: 85%;
		font-weight: 200;
	}
	.header__btn-md {
		display: none;
	}
	.header__right h1 {
		font-weight: 300;
	}
	.header__frames {
		position: absolute;
		top: 88vh;
		right: 44rem;
		transition: all 400ms ease;
	}
	.header__frame {
		width: 14rem;
		border: 0.1rem solid #eb9d2f;
		box-shadow: 0 0 4rem rgba(0, 0, 0, 0.5);
		position: absolute;
		transform: rotate(-10deg);
		transform-origin: bottom left;
		transition: all 400ms ease;
	}
	.header__frame:nth-child(2) {
		transform: rotate(20deg);
		top: -2rem;
		left: 2rem;
	}
	.header__frames:hover .header__frame {
		transform: rotate(0);
	}
	.header__frames:hover .header__frame:nth-child(2) {
		top: 0;
		left: 15rem;
	}
	@media screen and (max-width: 1024px) {
		header {
			height: fit-content;
			padding: 14rem 0 12rem;
			display: grid;
			place-items: center;
		}
		.header__image-bg {
			display: none;
		}
		.header__image-sm {
			display: none;
		}
		.header_container {
            grid-template-columns: 40% 54%;
            gap:6%;
            margin: 0;
		}
        .header__image-lg {
            filter: saturate(1) brightness(1);
            border: .1rem solid #eb9d2f;
            width: 100%;
            top: 0;
            left: 0;
        }
        .empty {
            display: none;
        }
        .header__right p{
            width: 100%;
        }
        .header__frames {
            display: none;
        }
        .header__tag {
            margin-bottom: 1rem;
        }
        .header__btn-md {
            background: #eb9d2f;
            color: azure;
            margin-top: 2rem;
            display: inline-block;
            padding: .6rem 1.6rem;
            font-weight: 600;
            border-radius: .3rem;
        }
	}
    @media screen and (max-width: 600px) {
        header {
            padding: 0;
            padding-bottom: 6rem;
        }
        .header_container{
            grid-template-columns: 1fr;
            gap: 1rem;
            text-align: center;
        }
        .header__image-lg{
          width: 80%;
          height: 20rem;
          margin: 0 auto;
          margin-top: 7rem;
          overflow: hidden;
          border-radius: 1rem;
        }
        .header__head {
            justify-content: center;
        }
        .header__right p {
            margin-top: 1rem;
        }
        /* .header__title {
            margin-top: 1rem;
        } */
        
    }
</style>
