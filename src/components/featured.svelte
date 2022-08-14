<section id="features">
	<div class="container exhibitions__container">
		<h2 class="exhibitions__title">Featured</h2>
		<div class="empty exhibtions__empty" />
		<div class="exhibitions__head">
			<p>
				Get access to a large variety of products ranging from healthcare to fashion at your nearest
				available stores.
			</p>
		</div>
		<div class="exhibitions__gallery">
			<article>
				<img src="/images/zgalleryC.jpg" alt="" />
				<p>Food Items</p>
			</article>
			<article>
				<img src="/images/zgalleryA.jpg" alt="" />
				<p>Groceries</p>
			</article>
			<article>
				<img src="/images/zgalleryB.jpg" alt="" />
				<p>Gift Items</p>
			</article>
			<article>
				<img src="/images/zgalleryE.jpg" alt="" />
				<p>Asthetics</p>
			</article>
			<article>
				<img src="/images/zgalleryD.jpg" alt="" />
				<p>Home Care</p>
			</article>
			<article>
				<img src="/images/zgalleryF.jpg" alt="" />
				<p>Fashion</p>
			</article>
			<article>
				<img src="/images/zgalleryG.jpg" alt="" />
				<p>Entertainment</p>
			</article>
		</div>
	</div>
</section>

<style>
	#features {
		margin-top: 7rem;
	}
	.exhibitions__container {
		position: relative;
	}
	.exhibtions__empty {
		width: 20rem;
		position: absolute;
		right: 14rem;
		top: 0;
	}
	.exhibitions__head {
		display: grid;
		grid-template-columns: auto 10rem;
		justify-content: space-between;
		align-items: center;
	}
	.exhibitions__head > p {
		width: 45rem;
		font-size: 0.8rem;
		letter-spacing: 1px;
	}
	.exhibitions__gallery {
		display: grid;
		grid-template-columns: repeat(3, 1fr);
		margin-top: 3rem;
		gap: 2rem;
	}
	.exhibitions__gallery article {
		transition: all 400ms ease;
		border: 0.1rem solid #eb9d2f;
	}
	.exhibitions__gallery article:nth-child(1) {
		grid-row: 1/3;
	}
	.exhibitions__gallery article:nth-child(4) {
		grid-column: 2/4;
		grid-row: 2/3;
	}
	.exhibitions__gallery article:nth-child(5) {
		height: 20rem;
	}
	.exhibitions__gallery article:nth-child(6) {
		height: 20rem;
	}
	.exhibitions__gallery article:nth-child(7) {
		height: 20rem;
	}
	.exhibitions__gallery article img {
		height: 100%;
		filter: saturate(0);
		transition: all 400ms ease;
		object-fit: cover;
	}
	.exhibitions__gallery article:hover img {
		filter: saturate(1);
	}
	.exhibitions__gallery article:hover {
		box-shadow: 0 4rem 4rem rgba(0, 0, 0, 0.5);
	}
	.exhibitions__gallery article > p {
		letter-spacing: 1px;
		font-size: 1rem;

		margin: 0.7rem 0.1rem;
	}

	@media screen and (max-width: 1024px) {
		.exhibitions__head > p {
			width: 100%;
			margin-top: 2rem;
		}
		.exhibitions__gallery {
			margin-top: 3rem;
			/* gap: 3rem; */
		}
		.exhibitions__gallery article {
			border: none;
		}
	}

	@media screen and (max-width: 600px) {
		#features {
			margin-top: 6rem;
		}
		.exhibitions__head {
			grid-template-columns: 1fr;
		}
		.exhibitions__head p {
			margin-top: 1rem;
		}
		.exhibitions__gallery {
			display: block;
		}
		.exhibitions__gallery article {
			width: 100%;
			height: fit-content;
			margin-bottom: 1rem;
		}
		.exhibitions__gallery article:nth-child(5) {
			height: fit-content;
		}
		.exhibitions__gallery article:nth-child(6) {
			height: fit-content;
		}
		.exhibitions__gallery article:nth-child(7) {
			height: fit-content;
		}
	}
</style>
