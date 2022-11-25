---
title: 首页
comments: false
toc: false
layout: homepage
---
<div class="activity-gallery">
    <div class="swiper-container">
        <div class="swiper-wrapper">
            <div class="swiper-slide init">
                <div class="inner">
                    <figure><img src="https://www.fairsandexpos.com/files/_cache/fb64cf8d3cf26eb58f5c0ae3348bcb5c.jpg"></figure>
                    <div class="gallery-item-desc">
                        <div class="typography-label">灵感迸发，一课又一课。</div>
                        <a href="/posts/test/">
                            <div class="typography-title">参加我们的实际操作互动课程</div>
                        </a>
                    </div>
                </div>
            </div>
            <div class="swiper-slide">
                <div class="inner">
                    <figure><img src="https://www.fairsandexpos.com/files/_cache/5553cc0ee6e1ca9311f1453775d8cc67.jpg"></figure>
                    <div class="gallery-item-desc">
                        <div class="typography-label">照片和视频</div>
                        <div class="typography-title">探索如何拍摄出你乐于分享的照片和视频。这里有“光影漫步”、“光影实验室”、“Pro 行家讲座”和“进阶讲座”等各种课程等你参加。</div>
                    </div>
                </div>
            </div>
            <div class="swiper-slide">
                <div class="inner">
                    <figure><img src="https://www.fairsandexpos.com/files/_cache/4c452b89fd37f07ea08bc6205e6e3800.png"></figure>
                    <div class="gallery-item-desc">
                        <div class="typography-label">音乐</div>
                        <div class="typography-title">你可以参加“进阶讲座”和“音乐实验室”等课程，开始创作属于自己的节拍；也可以参加“Pro 行家讲座”课程，让自己的音乐制作能力更进一步。</div>
                    </div>
                </div>
            </div>
            <div class="swiper-slide">
                <div class="inner">
                    <figure><img src="https://www.fairsandexpos.com/files/_cache/9989b389fdb3a3d23367fbe67663a9ee.png"></figure>
                    <div class="gallery-item-desc">
                        <div class="typography-title">来编写你的第一行代码，这比你想象的要容易多了。我们有“课外一小时”、“夏令营”、“进阶讲座”等各种课程，来教你学习如何编程。</div>
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
    swiper.$el.parent('.activity-gallery')[0].onmouseover = function() {
        swiper.$el.addClass('mouse-hover');
    };
    swiper.$el.parent('.activity-gallery')[0].onmouseout = function() {
        swiper.$el.removeClass('mouse-hover');
    };
</script>
