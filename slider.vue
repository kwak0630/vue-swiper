<template>
	<div>
		<Lnb />
		<div class="content slider-content">
			<h2>slider</h2>
			<p class="sub-tit">
				- vue swiper (slider) 연습
			</p>
			<div class="slider-wrap">
                <h6>slider 1 <span>(basic)</span></h6>
				<swiper
                    class="swiper"
                    :options="swiperOption"
                >
                    <swiper-slide>Slide 1</swiper-slide>     
                    <swiper-slide>Slide 2</swiper-slide>     
                    <swiper-slide>Slide 3</swiper-slide>     
                    <swiper-slide>Slide 4</swiper-slide>     
                    <swiper-slide>Slide 5</swiper-slide>
                    <div
                        class="swiper-pagination"
                        slot="pagination"
                        >
                    </div>
                    <div class="swiper-button-prev" slot="button-prev"></div>
                    <div class="swiper-button-next" slot="button-next"></div>
                </swiper>
			</div>
			<div class="slider-wrap">
                <h6>slider 2 <span>(center)</span></h6>
				<swiper
                    class="swiper"
                    :options="swiperOption2"
                >
                    <swiper-slide>Slide 1</swiper-slide>     
                    <swiper-slide>Slide 2</swiper-slide>     
                    <swiper-slide>Slide 3</swiper-slide>     
                    <swiper-slide>Slide 4</swiper-slide>     
                    <swiper-slide>Slide 5</swiper-slide>     
                    <swiper-slide>Slide 6</swiper-slide>     
                    <swiper-slide>Slide 7</swiper-slide>     
                    <swiper-slide>Slide 8</swiper-slide>     
                    <swiper-slide>Slide 9</swiper-slide>     
                    <swiper-slide>Slide 10</swiper-slide>     
                    <div
                        class="swiper-pagination"
                        slot="pagination"
                        >
                    </div>
                    <div class="swiper-button-prev" slot="button-prev"></div>
                    <div class="swiper-button-next" slot="button-next"></div>
                </swiper>
			</div>
			<div class="slider-wrap">
                <h6>slider 3 <span>(progress bar)</span></h6>
				<swiper
                    class="swiper"
                    :options="swiperOption3"
                >
                    <swiper-slide>Slide 1</swiper-slide>     
                    <swiper-slide>Slide 2</swiper-slide>     
                    <swiper-slide>Slide 3</swiper-slide>     
                    <swiper-slide>Slide 4</swiper-slide>     
                    <swiper-slide>Slide 5</swiper-slide>  
                    <div
                        class="swiper-pagination"
                        slot="pagination"
                        >
                    </div>
                    <div
                        class="swiper-progress"
                        :class="{start: startProgress}"
                        slot="pagination"
                        >
                        <div class="bar"></div>
                    </div>
                </swiper>
			</div>
			<div class="slider-wrap">
                <h6>slider 4 <span>(custom pagination)</span></h6>
				<swiper
                    class="swiper"
                    :options="swiperOption4"
                >
                    <swiper-slide>Slide 1</swiper-slide>     
                    <swiper-slide>Slide 2</swiper-slide>     
                    <swiper-slide>Slide 3</swiper-slide>     
                    <swiper-slide>Slide 4</swiper-slide>     
                    <swiper-slide>Slide 5</swiper-slide>  
                    <div
                        class="swiper-pagination num"
                        slot="pagination"
                        >
                    </div>
                </swiper>
			</div>
			<div class="slider-wrap">
                <h6>slider 5 <span>(vertical)</span></h6>
				<swiper
                    class="swiper"
                    :options="swiperOption5"
                >
                    <swiper-slide>Slide 1</swiper-slide>     
                    <swiper-slide>Slide 2</swiper-slide>     
                    <swiper-slide>Slide 3</swiper-slide>     
                    <swiper-slide>Slide 4</swiper-slide>     
                    <swiper-slide>Slide 5</swiper-slide>
                    <div
                        class="swiper-pagination"
                        slot="pagination"
                        >
                    </div>
                </swiper>
			</div>
			<div class="slider-wrap">
                <h6>slider 6 <span>(effect)</span></h6>
				<swiper
                    class="swiper"
                    :options="swiperOption6"
                >
                    <swiper-slide>Slide 1</swiper-slide>     
                    <swiper-slide>Slide 2</swiper-slide>     
                    <swiper-slide>Slide 3</swiper-slide>     
                    <swiper-slide>Slide 4</swiper-slide>     
                    <swiper-slide>Slide 5</swiper-slide>
                    <div
                        class="swiper-pagination"
                        slot="pagination"
                        >
                    </div>
                </swiper>
			</div>
			<div class="slider-wrap">
                <h6>slider 7 <span>(freeMode)</span></h6>
				<swiper
                    class="swiper"
                    :options="swiperOption7"
                >
                    <swiper-slide>Slide 1</swiper-slide>     
                    <swiper-slide>Slide 2</swiper-slide>     
                    <swiper-slide>Slide 3</swiper-slide>     
                    <swiper-slide>Slide 4</swiper-slide>     
                    <swiper-slide>Slide 5</swiper-slide>
                    <div
                        class="swiper-pagination"
                        slot="pagination"
                        >
                    </div>
                </swiper>
			</div>
			<div class="slider-wrap">
                <h6>slider 8 <span>(side)</span></h6>
				<swiper
                    class="swiper"
                    :options="swiperOption8"
                >
                    <swiper-slide>Slide 1</swiper-slide>     
                    <swiper-slide>Slide 2</swiper-slide>     
                    <swiper-slide>Slide 3</swiper-slide>     
                    <swiper-slide>Slide 4</swiper-slide>     
                    <swiper-slide>Slide 5</swiper-slide>     
                    <swiper-slide>Slide 6</swiper-slide>     
                    <swiper-slide>Slide 7</swiper-slide>     
                    <swiper-slide>Slide 8</swiper-slide>     
                    <swiper-slide>Slide 9</swiper-slide>     
                    <swiper-slide>Slide 10</swiper-slide>     
                    <div
                        class="swiper-pagination"
                        slot="pagination"
                        >
                    </div>
                    <div class="swiper-button-prev" slot="button-prev"></div>
                    <div class="swiper-button-next" slot="button-next"></div>
                </swiper>
			</div>
			<div class="slider-wrap thumb-example">
                <h6>slider 9 <span>(thumb)</span></h6>
                <swiper class="swiper gallery-top" :options="swiperOptionTop" ref="swiperTop">
                    <swiper-slide class="slide-1">1</swiper-slide>
                    <swiper-slide class="slide-2">2</swiper-slide>
                    <swiper-slide class="slide-3">3</swiper-slide>
                    <swiper-slide class="slide-4">4</swiper-slide>
                    <swiper-slide class="slide-5">5</swiper-slide>
                    <swiper-slide class="slide-6">6</swiper-slide>
                    <div class="swiper-button-next" slot="button-next"></div>
                    <div class="swiper-button-prev" slot="button-prev"></div>
                </swiper>

                <swiper class="swiper gallery-thumbs" :options="swiperOptionThumbs" ref="swiperThumbs">
                    <swiper-slide class="slide-1">1</swiper-slide>
                    <swiper-slide class="slide-2">2</swiper-slide>
                    <swiper-slide class="slide-3">3</swiper-slide>
                    <swiper-slide class="slide-4">4</swiper-slide>
                    <swiper-slide class="slide-5">5</swiper-slide>
                    <swiper-slide class="slide-6">6</swiper-slide>
                </swiper>
			</div>
		</div>
		<Footer />
	</div>
</template>

<script>
	import Lnb from "@/components/layout/Lnb";
	import Footer from "@/components/layout/Footer";
    import { Swiper, SwiperSlide } from "vue-awesome-swiper";
    import "swiper/css/swiper.css";

	export default {
		name: "slider",
		components:	{
			Lnb,
			Footer,
            Swiper,
            SwiperSlide
		},
		props: {
			
		},
		data() {
			return {
				swiperOption: { 
                    slidesPerView: 1, 
                    spaceBetween: 30, 
                    loop: true, 
                    pagination: { 
                        el: '.swiper-pagination', 
                        clickable: true,
                    }, 
                    navigation: { 
                        nextEl: '.swiper-button-next', 
                        prevEl: '.swiper-button-prev' 
                    } 
                },

                swiperOption2: {
                    centeredSlides: true,
                    autoplay: {
                        delay: 3000
                    },
                    slidesPerView: 3, 
                    spaceBetween: 30, 
                    loop: true, 
                    pagination: { 
                        el: '.swiper-pagination', 
                        clickable: true 
                    }, 
                },

                startProgress: false,
                swiperOption3: {
                    loop: true,
                    threshold: 20,
                    autoplay: {
                        delay: 5000
                    },
                    on: {
                        init: this.init,
                        sliderMove: this.stopAutoplay,
                        sliderChaneTransitionStart: this.stopAutoplay,
                        transitionEnd: this.startAutoplay
                    },
                    pagination: {
                        el: ".swiper-pagination",
                        clickable: true
                    }
                },

                swiperOption4: {
                    slidesPerView: 1,
                    autoplay: {
                        delay: 5000
                    },
                    pagination: {
                        el: ".swiper-pagination",
                        type: "fraction",
                        disabledClass: 'disabled'
                    },
                },

				swiperOption5: { 
                    direction: 'vertical',
                    slidesPerView: 1, 
                    spaceBetween: 30, 
                    loop: true, 
                    pagination: { 
                        el: '.swiper-pagination', 
                        clickable: true 
                    }, 
                },

				swiperOption6: { 
                    effect: 'covecuberflow',
                    autoplay: {
                        delay: 3000
                    },
                    slidesPerView: 1, 
                    loop: true, 
                    pagination: { 
                        el: '.swiper-pagination', 
                        clickable: true 
                    }, 
                },

				swiperOption7: { 
                    freeMode: true,
                    autoplay: {
                        delay: 3000
                    },
                    slidesPerView: 3, 
                    spaceBetween: 30, 
                    loop: true, 
                    pagination: { 
                        el: '.swiper-pagination', 
                        clickable: true 
                    }, 
                },

                swiperOption8: {
                    autoplay: {
                        delay: 3000
                    },
                    slidesPerView: 2.5, 
                    spaceBetween: 30, 
                    loop: true, 
                    pagination: { 
                        el: '.swiper-pagination', 
                        clickable: true 
                    }, 
                },

                swiperOptionTop: {
                    autoplay: {
                        delay: 3000
                    },
                    effect: 'fade',
                    loop: true,
                    loopedSlides: 5,
                    spaceBetween: 10,
                    navigation: {
                        nextEl: '.swiper-button-next',
                        prevEl: '.swiper-button-prev'
                    }
                },
                swiperOptionThumbs: {
                    loop: true,
                    loopedSlides: 5,
                    spaceBetween: 10,
                    centeredSlides: true,
                    slidesPerView: 'auto',
                    touchRatio: 0.2,
                    slideToClickedSlide: true
                }
			};
		},
		computed: {
		},
		methods: {
            init() {
                this.startProgress = true
            },
            stopAutoplay() {
                try {
                    this.swiper.autoplay.stop()
                    this.startProgress = false
                } catch (err) {
                    //console.error(err)
                }
            },
            startAutoplay() {
                try {
                    this.swiper.autoplay.start()
                    this.startProgress = true
                } catch (err) {
                    //console.error(err)
                }
            },
		},
		watch: {
			
		},
        mounted() {
            this.$nextTick(() => {
                const swiperTop = this.$refs.swiperTop.$swiper
                const swiperThumbs = this.$refs.swiperThumbs.$swiper
                swiperTop.controller.control = swiperThumbs
                swiperThumbs.controller.control = swiperTop
            })
        }
	}
</script>
<style lang="scss">
.slider-content{
    padding-bottom:170px;
}
.slider-wrap{
    h6{
        font-size:24px;
        margin-bottom:20px;
    }
    &+.slider-wrap{
        margin-top:40px;
    }
    &.thumb-example {
        height: 480px;
        .swiper-slide {
            display: flex; 
            justify-content: center; 
            align-items: center; 
            text-align: center; 
            font-weight: bold; 
            background-size: cover;
            background-position: center;
            &.slide-1 {
                background-image:url('~@/assets/img01.jpg');
            }
            &.slide-2 {
                background-image:url('~@/assets/img02.png');
            }
            &.slide-3 {
                background-image:url('~@/assets/img01.jpg');
            }
            &.slide-4 {
                background-image:url('~@/assets/img02.png');
            }
            &.slide-5 {
                background-image:url('~@/assets/img01.jpg');
            }
            &.slide-6 {
                background-image:url('~@/assets/img02.png');
            }
        }
        .gallery-top {
            height: 80%;
            width: 100%;
        }
        .gallery-thumbs {
            height: 20%;
            margin-top:20px;
        }
        .gallery-thumbs .swiper-slide {
            width: 25%;
            height: 100%;
            opacity: 0.4;
        }
        .gallery-thumbs .swiper-slide-active {
            opacity: 1;
        }
    }
} 
.swiper { 
    width: 100%; 
    height: 300px; 
    .swiper-slide { 
        display: flex; 
        justify-content: center; 
        align-items: center; 
        text-align: center; 
        font-weight: bold; 
        background:#fdde88;
        opacity: 0.7;
        img{
            width:100%
        }
        &.swiper-slide-active{
            opacity: 1;
        }
    }
    .swiper-pagination{
        bottom:20px;
        &.num{
            display:inline-block;
            width:auto;
            left:20px;
            padding:7px 15px;
            background:#fff;
            border-radius: 20px;
            color:#666;
            .swiper-pagination-current{
                font-weight:900;
                color:#ff7600
            }
            .swiper-pagination-total{
                color:#666
            }
        }
    }
    .swiper-progress{
        position:absolute;
        bottom:0;
        left:0;
        width:100%;
        z-index: 1;
        background:#333;
        .bar{
            width:100%;
            height:4px;
            transform: translateX(-100%);
            background:#ff7600;
        }
        &.start{
            .bar{
                animation-duration: 5s;
                animation-iteration-count: infinite;
                animation-name: progress;
            }
        }
    }
}

@keyframes progress {
    from {
        transform: translateX(-100%);
    }
    to {
        transform: translateX(0);
    }
}

</style>