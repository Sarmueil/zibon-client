<script lang="ts">
	import { Swiper, SwiperSlide } from 'swiper/svelte';
	import 'swiper/css';
	import 'swiper/css/pagination';
	import { Pagination } from 'swiper';
</script>

<section id="gallery">
	<div class="container gallery__container">
		<div class="gallery__head">
			<h2 class="gallery__title">Featured Products</h2>
			<div class="empty gallery__empty" />
		</div>
		<p>
			Lorem, ipsum dolor sit amet consectetur adipisicing elit. Sit minima non ipsam perspiciatis
			incidunt? Ad ipsum dignissimos ipsam a non.
		</p>

		<div class="swiper__wrapper">
			<Swiper
				slidesPerView={4}
				spaceBetween={20}
				pagination={{
					clickable: true
				}}
                 breakpoints={{
                    "599 ": {
                      slidesPerView: 2,
                      spaceBetween: 40,
                    },
                    "1023": {
                      slidesPerView: 4,
                      spaceBetween: 50,
                    },
                  }}
				modules={[Pagination]}
				class="mySwiper"
			>
				<SwiperSlide>
					<div class="swiper__flex">
						<img src="/images/aboutZibon.jpg" alt="" />
						<p class="swiper__text">Fasshion</p>
					</div>
				</SwiperSlide>
				<SwiperSlide>
					<div class="swiper__flex">
						<img src="/images/aboutZibon.jpg" alt="" />
						<p class="swiper__text">Fasshion</p>
					</div>
				</SwiperSlide>
				<SwiperSlide>
					<div class="swiper__flex">
						<img src="/images/aboutZibon.jpg" alt="" />
						<p class="swiper__text">Fasshion</p>
					</div>
				</SwiperSlide>
				<SwiperSlide>
					<div class="swiper__flex">
						<img src="/images/aboutZibon.jpg" alt="" />
						<p class="swiper__text">Fasshion</p>
					</div>
				</SwiperSlide>
                <SwiperSlide>
                    <div class="swiper__flex">
                        <img src="/images/aboutZibon.jpg" alt="">
                        <p class="swiper__text">Fasshion</p>
                    </div>
                </SwiperSlide>
                <SwiperSlide>
                    <div class="swiper__flex">
                        <img src="/images/aboutZibon.jpg" alt="">
                        <p class="swiper__text">Fasshion</p>
                    </div>
                </SwiperSlide>
                  <SwiperSlide>
                    <div class="swiper__flex">
                        <img src="/images/aboutZibon.jpg" alt="">
                        <p class="swiper__text">Fasshion</p>
                    </div>
                </SwiperSlide>
			</Swiper>
		</div>
	</div>
</section>

<style>
	#gallery {
		margin-top: 12rem;
	}
	.gallery__head {
		display: flex;
		justify-content: space-between;
	}
	.gallery__container p {
		width: 45rem;
	}
	.swiper__wrapper {
		margin-top: 5rem;
		height: 20rem;
		padding-bottom: 4rem;
	}
	.swiper__flex {
		display: flex;
        flex-direction: column;
		align-items: center;
	}
	.swiper__text {
		color: white;
	}
</style>
