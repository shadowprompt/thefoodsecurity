---
title: 首页
comments: false
---
<div class="apple-retail">
    <div class="swiper-container">
        <div class="swiper-wrapper">
            <div class="swiper-slide init">
                <div class="inner">
                    <figure><img src="/swiper/images/carousel01.png"></figure>
                    <div class="gallery-item-desc">
                        <h3 class="typography-label">灵感迸发，一课又一课。</h3>
                        <p class="typography-body">参加我们的实际操作互动课程，与影响广泛的艺术家、音乐家、开发者和企业家开展交流。</p>
                    </div>
                </div>
            </div>
            <div class="swiper-slide">
                <div class="inner">
                    <figure><img src="/swiper/images/carousel01.png"></figure>
                    <div class="gallery-item-desc">
                        <h3 class="typography-label">照片和视频</h3>
                        <p class="typography-body">探索如何拍摄出你乐于分享的照片和视频。这里有“光影漫步”、“光影实验室”、“Pro 行家讲座”和“进阶讲座”等各种课程等你参加。</p>
                    </div>
                </div>
            </div>
            <div class="swiper-slide">
                <div class="inner">
                    <figure><img src="/swiper/images/carousel01.png"></figure>
                    <div class="gallery-item-desc">
                        <h3 class="typography-label">音乐</h3>
                        <p class="typography-body">你可以参加“进阶讲座”和“音乐实验室”等课程，开始创作属于自己的节拍；也可以参加“Pro 行家讲座”课程，让自己的音乐制作能力更进一步。</p>
                    </div>
                </div>
            </div>
            <div class="swiper-slide">
                <div class="inner">
                    <figure><img src="/swiper/images/carousel01.png"></figure>
                    <div class="gallery-item-desc">
                        <h3 class="typography-label">编程</h3>
                        <p class="typography-body">来编写你的第一行代码，这比你想象的要容易多了。我们有“课外一小时”、“夏令营”、“进阶讲座”等各种课程，来教你学习如何编程。</p>
                    </div>
                </div>
            </div>
            <div class="swiper-slide">
                <div class="inner">
                    <figure><img src="/swiper/images/carousel01.png"></figure>
                    <div class="gallery-item-desc">
                        <h3 class="typography-label">艺术和设计</h3>
                        <p class="typography-body">参加我们的“现场艺术创作”、“户外写生”、“课外一小时”和“进阶讲座”等课程，开始你的新创作。</p>
                    </div>
                </div>
            </div>
        </div>
        <div class="swiper-button-prev"></div>
        <!--左箭头-->
        <div class="swiper-button-next"></div>
        <!--右箭头-->
    </div>
</div>

<script>
    var swiper = new Swiper('.swiper-container', {
        speed: 700,
        slidesPerView: 'auto',
        centeredSlides: true,
        autoplay:true,
        loop: true,
        on: {
            init: function() {
                this.slides.removeClass('init');
            },
        },
        navigation: {
            nextEl: '.swiper-button-next',
            prevEl: '.swiper-button-prev',
        },

    });
    swiper.$el.parent('.apple-retail')[0].onmouseover = function() {
        swiper.$el.addClass('mouse-hover');
    };
    swiper.$el.parent('.apple-retail')[0].onmouseout = function() {
        swiper.$el.removeClass('mouse-hover');
    };
</script>
