<footer id="download">
	<div class="container footer__container">
		<div class="footer__head">
			<h2 class="footer__title">Try Zibon Today</h2>
			<div class="footer__logo">
				<img src="/images/zibonLogo.png" alt="Header_logo" class="nav__logo" />
			</div>
		</div>
		<div class="app__download-container">
			<p>The one stop app for safe and secure purchase of your items</p>
			<ul class="nav__socials">
				<li><a href="/"><i class="uil uil-instagram-alt" /></a></li>
				<li><a href="/"><i class="uil uil-twitter" /></a></li>
				<li><a href="/"><i class="uil uil-instagram-alt" /></a></li>
			</ul>
	
			<div class="footer__links-frames">
              <article><img src="/images/google.png" alt=""></article>
              <article><img src="/images/apple.png" alt=""></article>
            </div>
		</div>
		<ul class="footer__links">
			<li><a href="/">Home</a></li>
			<li><a href="/">About</a></li>
			<li><a href="/">SiteMap</a></li>
			<li><a href="/">Privacy Policy</a></li>
		</ul>
	</div>
</footer>

<style>
	footer {
		margin-top: 7rem;
	}
	.footer__container {
		border-top: 0.3rem solid #eb9d2f;
		padding-top: 5rem;
		/* width: 80%; */
	}
	.footer__head {
		display: flex;
		align-items: center;
		gap: 2rem;
	}
	.footer__links {
		margin: 2rem 0 4rem;
		display: flex;
		align-items: center;
		gap: 5rem;
        font-size: .7rem;
	}
	.app__download-container {
		margin-top: 1rem;
	}
	.nav__logo {
		width: 7.5rem;
	}
	.footer__logo {
		padding: 0.5rem;
		border: 0.2rem solid #eb9d2f;
	}
    .app__download-container p {
        font-size: .9rem;
        letter-spacing: 2px;
    }
    .footer__links-frames {
        display: flex;
        align-items: center;
    }
    .footer__links-frames article {
       width: 13rem;
    }
	.nav__socials {
		display: none;
		gap: 1rem;
		margin-top: .7rem;
	}
	.nav__socials a {
		width: 2rem;
		height: 2rem;
		display: grid;
		background-color: #eb9d2f;
		border-radius: 0.5rem;
		color: #243b55;
		place-items: center;
	}
	.nav__socials a:hover {
		box-shadow: 0 1rem 1rem rgba(0, 0, 0, 0.4);
	}

	@media screen and (max-width: 600px) {
		/* .footer__head {
			flex-direction: column;
		} */
		.footer__head h2 {
			font-size: 1.5rem;
		}
		.footer__links {
			flex-direction: column;
			gap: 2rem;
			margin-top: 5rem;
		}
		.app__download-container {
			margin-top: 1rem;
		}
		.app__download-container p {
			font-size: .8rem;
		}
		.nav__socials {
			display: flex;
		}
	}
</style>
