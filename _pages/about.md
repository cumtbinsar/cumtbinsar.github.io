---
permalink: /
title: "InSAR Geohazard Team @ CUMTB"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

**中国矿业大学（北京）· 地表形变与地质灾害研究团队**

## 团队简介

<style>
  .homepage-carousel {
    position: relative;
    width: 100%;
    aspect-ratio: 16 / 9;
    margin: 1.5rem auto;
    overflow: hidden;
    border-radius: 8px;
    box-shadow: 0 8px 24px rgba(0, 0, 0, 0.14);
  }

  .homepage-carousel > img {
    position: absolute;
    inset: 0;
    display: block;
    width: 100%;
    height: 100%;
    object-fit: cover;
    opacity: 0;
    pointer-events: none;
    transition: opacity 0.35s ease;
  }

  .homepage-carousel > img.is-active {
    opacity: 1;
    pointer-events: auto;
  }

  .homepage-carousel__button {
    position: absolute;
    top: 50%;
    z-index: 2;
    width: 2.5rem;
    height: 2.5rem;
    border: 0;
    border-radius: 50%;
    color: #fff;
    background: rgba(0, 0, 0, 0.45);
    line-height: 1;
    transform: translateY(-50%);
    cursor: pointer;
    transition: background 0.2s ease;
  }

  .homepage-carousel__button:hover,
  .homepage-carousel__button:focus-visible {
    background: rgba(0, 0, 0, 0.65);
  }

  .homepage-carousel__button--prev {
    left: 0.75rem;
  }

  .homepage-carousel__button--next {
    right: 0.75rem;
  }

  .homepage-carousel__dots {
    position: absolute;
    right: 0;
    bottom: 0.75rem;
    left: 0;
    z-index: 2;
    display: flex;
    justify-content: center;
    gap: 0.55rem;
  }

  .homepage-carousel__dot {
    width: 0.7rem;
    height: 0.7rem;
    padding: 0;
    border: 1px solid rgba(255, 255, 255, 0.9);
    border-radius: 50%;
    background: rgba(255, 255, 255, 0.35);
    cursor: pointer;
    transition: background 0.2s ease, transform 0.2s ease;
  }

  .homepage-carousel__dot.is-active {
    background: #fff;
    transform: scale(1.15);
  }
</style>

<div class="homepage-carousel" aria-label="主页图片轮播">
  <img class="is-active" src="/files/homepage0.jpg" alt="团队主页图片 1">
  <img src="/files/homepage1.jpg" alt="团队主页图片 2">
  <img src="/files/homepage2.jpg" alt="团队主页图片 3">
  <img src="/files/homepage3.jpg" alt="团队主页图片 4">

  <button class="homepage-carousel__button homepage-carousel__button--prev" type="button" aria-label="上一张">‹</button>
  <button class="homepage-carousel__button homepage-carousel__button--next" type="button" aria-label="下一张">›</button>

  <div class="homepage-carousel__dots" aria-label="选择轮播图片">
    <button class="homepage-carousel__dot is-active" type="button" aria-label="第 1 张"></button>
    <button class="homepage-carousel__dot" type="button" aria-label="第 2 张"></button>
    <button class="homepage-carousel__dot" type="button" aria-label="第 3 张"></button>
    <button class="homepage-carousel__dot" type="button" aria-label="第 4 张"></button>
  </div>
</div>



<script>
  (() => {
    const carousel = document.querySelector('.homepage-carousel');
    if (!carousel) {
      return;
    }

    const slides = Array.from(carousel.querySelectorAll(':scope > img'));
    const dots = Array.from(carousel.querySelectorAll('.homepage-carousel__dot'));
    const previousButton = carousel.querySelector('.homepage-carousel__button--prev');
    const nextButton = carousel.querySelector('.homepage-carousel__button--next');
    let activeIndex = Math.max(0, slides.findIndex((slide) => slide.classList.contains('is-active')));
    let autoplayId;

    const showSlide = (nextIndex) => {
      slides[activeIndex].classList.remove('is-active');
      dots[activeIndex].classList.remove('is-active');
      activeIndex = (nextIndex + slides.length) % slides.length;
      slides[activeIndex].classList.add('is-active');
      dots[activeIndex].classList.add('is-active');
    };

    const startAutoplay = () => {
      window.clearInterval(autoplayId);
      autoplayId = window.setInterval(() => showSlide(activeIndex + 1), 5000);
    };

    const handleManualChange = (nextIndex) => {
      showSlide(nextIndex);
      startAutoplay();
    };

    previousButton.addEventListener('click', () => handleManualChange(activeIndex - 1));
    nextButton.addEventListener('click', () => handleManualChange(activeIndex + 1));
    dots.forEach((dot, index) => {
      dot.addEventListener('click', () => handleManualChange(index));
    });

    startAutoplay();
  })();
</script>


唐伟，副教授，博士生导师。武汉大学测绘遥感信息工程国家重点实验室博士毕业，德国地学研究中心 GFZ 博士后（CSC-DAAD 博士后奖学金），德国汉诺威大学高级访问学者（DAAD 奖学金）。长期从事空间大地测量与遥感技术（SAR/InSAR/GNSS）在地质灾害、地下水资源管理、生态环境变化及地球物理建模等领域的应用研究。团队成员的研究方向主要涵盖大地测量技术、地表形变灾害监测与风险评估、地下水资源可持续利用等。通过融合多源遥感观测与数值模拟，我们致力于为城市地下水管理、地质灾害监测与预警、地质环境变化分析等提供关键的理论依据与技术支撑。

已发表SCI论文40余篇。相关论文发表在Remote Sensing of Environment、International Journal of Rock Mechanics and Mining Sciences、Journal of Hydrology、《地球物理学报》等行业知名期刊，研究成果受到了社会关注，被相关媒体追踪报道。主持国家自然科学基金面上项目1项、青年基金C类项目1项、国家自然科学基金科技活动项目（科学传播类）1项、国家重点研发计划“政府间国际科技创新合作”项目课题1项。

**研究方向**  
- 空间大地测量技术：包括 SAR/InSAR 时序分析、GNSS 监测及多源数据融合方法。  
- 地表形变灾害监测与风险评估：涵盖地面沉降、滑坡、采空区沉陷、露天矿边坡等地质灾害的监测与分析。  
- 超采含水层地面沉降研究：利用多源大地测量与遥感观测，结合数值模拟开展地下水超采引发的地面沉降机理分析与地下水资源可持续管理研究。  
- 地球物理建模与参数反演：面向地下资源开采的力学—水文—地球物理耦合建模及参数反演方法开发。

**电子邮箱**：[weitang@cumtb.edu.cn](mailto:weitang@cumtb.edu.cn)

---

## InSAR Geohazard Team

**The InSAR Geohazard Team at CUMTB**, led by **Associate Professor Wei Tang** at China University of Mining and Technology (Beijing), focuses on advanced geodetic and remote sensing technologies for understanding and mitigating Earth surface hazards. Our research integrates **SAR/InSAR, GNSS, multi-source Earth observation, and numerical modeling** to investigate geohazards, groundwater resources, geo-environment change, and crustal deformation processes.

Our team’s research directions include:  
- Advanced geodetic technologies (InSAR, GNSS, time-series analysis)  
- Surface deformation and geohazard monitoring, including land subsidence, landslides, and mining-induced ground movement  
- Groundwater sustainability assessment and aquifer deformation analysis  
- Eco-environmental change detection using multi-sensor remote sensing data  
- Numerical modeling and geophysical interpretation for deformation mechanisms and disaster risk evaluation  

By combining multi-source satellite data with geomechanical and hydrological modeling, our team provides essential scientific insights and technological support for urban groundwater management, geohazard early warning, and geo-environmental monitoring. We aim to contribute innovative methodologies and decision-support tools to promote sustainable urban development and regional environmental security.
