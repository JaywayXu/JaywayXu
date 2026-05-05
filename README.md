<!-- ================= Research Highlights Carousel Start ================= -->

<style>
.research-carousel-wrapper {
  width: 100%;
  margin: 28px auto 42px auto;
  position: relative;
}

.research-carousel {
  position: relative;
  width: 100%;
  height: 430px;
  overflow: hidden;
  border-radius: 18px;
  box-shadow: 0 12px 32px rgba(0, 0, 0, 0.16);
  background: #f5f5f5;
  -webkit-user-select: none;
  user-select: none;
  touch-action: pan-y;
}

.research-carousel-track {
  display: flex;
  height: 100%;
  transform: translate3d(0, 0, 0);
  transition: transform 1050ms cubic-bezier(0.22, 0.61, 0.36, 1);
  will-change: transform;
  backface-visibility: hidden;
}

.research-carousel-slide {
  min-width: 100%;
  height: 100%;
  position: relative;
  overflow: hidden;
  transform: translateZ(0);
  backface-visibility: hidden;
}

.research-carousel-slide img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  object-position: center;
  display: block;
  pointer-events: none;
  transform: scale(1.035);
  transition:
    transform 1600ms cubic-bezier(0.22, 0.61, 0.36, 1),
    opacity 900ms ease;
  will-change: transform;
  backface-visibility: hidden;
}

.research-carousel-slide.active img {
  transform: scale(1);
}

.research-carousel-caption {
  position: absolute;
  left: 0;
  right: 0;
  bottom: 0;
  padding: 26px 34px;
  color: #fff;
  background: linear-gradient(
    to top,
    rgba(0, 0, 0, 0.72),
    rgba(0, 0, 0, 0.38),
    rgba(0, 0, 0, 0)
  );
  opacity: 0;
  transform: translate3d(0, 18px, 0);
  transition:
    opacity 850ms ease 220ms,
    transform 850ms cubic-bezier(0.22, 0.61, 0.36, 1) 220ms;
  will-change: opacity, transform;
}

.research-carousel-slide.active .research-carousel-caption {
  opacity: 1;
  transform: translate3d(0, 0, 0);
}

.research-carousel-caption h3 {
  margin: 0 0 10px 0;
  font-size: 24px;
  font-weight: 700;
  line-height: 1.3;
  color: #fff;
}

.research-carousel-caption p {
  margin: 0;
  font-size: 16px;
  line-height: 1.65;
  max-width: 850px;
  color: #fff;
  font-weight: 600;
}

.research-carousel-btn {
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  width: 42px;
  height: 42px;
  border: none;
  border-radius: 50%;
  background: rgba(0, 0, 0, 0.42);
  color: #fff;
  font-size: 24px;
  cursor: pointer;
  z-index: 5;
  transition:
    background 250ms ease,
    transform 250ms ease,
    opacity 250ms ease;
}

.research-carousel-btn:hover,
.research-carousel-btn:focus {
  background: rgba(0, 0, 0, 0.68);
  outline: none;
}

.research-carousel-btn.prev {
  left: 16px;
}

.research-carousel-btn.next {
  right: 16px;
}

.research-carousel-dots {
  display: flex;
  justify-content: center;
  gap: 9px;
  margin-top: 14px;
}

.research-carousel-dot {
  width: 10px;
  height: 10px;
  border-radius: 50%;
  border: none;
  background: #c9c9c9;
  cursor: pointer;
  transition:
    width 280ms ease,
    background 280ms ease,
    transform 280ms ease;
  padding: 0;
}

.research-carousel-dot.active {
  width: 26px;
  border-radius: 999px;
  background: #3b82f6;
}

.research-carousel-dot:hover {
  transform: scale(1.15);
}

.research-carousel-dot:focus {
  outline: 2px solid rgba(59, 130, 246, 0.45);
  outline-offset: 3px;
}

/* 尊重系统“减少动态效果”的设置 */
@media (prefers-reduced-motion: reduce) {
  .research-carousel-track,
  .research-carousel-slide img,
  .research-carousel-caption,
  .research-carousel-dot,
  .research-carousel-btn {
    transition: none;
  }

  .research-carousel-slide img {
    transform: scale(1);
  }
}

/* 移动端适配 */
@media (max-width: 768px) {
  .research-carousel {
    height: 260px;
    border-radius: 12px;
  }

  .research-carousel-caption {
    padding: 18px 20px;
  }

  .research-carousel-caption h3 {
    font-size: 18px;
  }

  .research-carousel-caption p {
    font-size: 13px;
    line-height: 1.45;
  }

  .research-carousel-btn {
    width: 34px;
    height: 34px;
    font-size: 20px;
  }
}
</style>

<div class="research-carousel-wrapper">
  <div class="research-carousel" id="researchCarousel">
    <div class="research-carousel-track">

      <div class="research-carousel-slide"> 
        <img src="images/carousel/Gary_wust.jpg" alt="Welcome Professor Gary G. Yen">
        <div class="research-carousel-caption">
          <h3>Warmly Welcome IEEE Fellow Professor Gary G. Yen to Visit Our Research Group in 2025</h3>
          <p>
            It is a great honor for our research group to welcome Professor Gary G. Yen, IEEE Fellow,
            for academic exchange and scholarly discussion.
          </p>
        </div>
      </div>

      <div class="research-carousel-slide"> 
        <img src="images/carousel/Ishibuchi_wust.jpg" alt="Welcome Professor Hisao Ishibuchi">
        <div class="research-carousel-caption">
          <h3>Warmly Welcome IEEE Fellow Professor Hisao Ishibuchi to Visit Our Research Group in 2025</h3>
          <p>
            It is a great honor for our research group to welcome Professor Hisao Ishibuchi, IEEE Fellow,
            for academic exchange and scholarly discussion.
          </p>
        </div>
      </div>

      <div class="research-carousel-slide"> 
        <img src="images/carousel/BICTA25.jpg" alt="BICTA 2025 Group Photo">
        <div class="research-carousel-caption">
          <h3>Our Research Group Co-organized BICTA 2025</h3>
          <p>
            As a co-organizer of BICTA 2025, our research group actively supported scholarly
            exchange and interdisciplinary collaboration in bio-inspired computing,
            evolutionary computation, and intelligent optimization.
          </p>
        </div>
      </div>

      <div class="research-carousel-slide"> 
        <img src="images/carousel/TY.jpg" alt="Welcome Professor Ye Tian">
        <div class="research-carousel-caption">
          <h3>Warmly Welcome Professor Ye Tian to Visit Our Research Group in 2025</h3>
          <p>
            It is a great honor for our research group to welcome Professor Ye Tian
            for academic exchange and scholarly discussion.
          </p>
        </div>
      </div>

      <div class="research-carousel-slide"> 
        <img src="images/carousel/23_Gary_wust.jpg" alt="Welcome Professor Gary G. Yen in 2023">
        <div class="research-carousel-caption">
          <h3>Warmly Welcome IEEE Fellow Professor Gary G. Yen to Visit Our Research Group in 2023</h3>
          <p>
            It is a great honor for our research group to welcome Professor Gary G. Yen, IEEE Fellow,
            for academic exchange and scholarly discussion.
          </p>
        </div>
      </div>

    </div>

    <button class="research-carousel-btn prev" type="button" aria-label="Previous slide">&#10094;</button>
    <button class="research-carousel-btn next" type="button" aria-label="Next slide">&#10095;</button>
  </div>

  <div class="research-carousel-dots" id="researchCarouselDots"></div>
</div>

<script>
(function () {
  function initResearchCarousel() {
    const carousel = document.getElementById("researchCarousel");
    if (!carousel) return;

    /*
     * 防止重复初始化。
     * 如果脚本被浏览器缓存恢复、Jekyll 页面重载或其他机制重复执行，
     * 先销毁旧实例，避免多个定时器叠加导致轮播突然变快。
     */
    if (
      carousel.__researchCarouselInstance &&
      typeof carousel.__researchCarouselInstance.destroy === "function"
    ) {
      carousel.__researchCarouselInstance.destroy();
    }

    const wrapper = carousel.closest(".research-carousel-wrapper") || carousel;
    const track = carousel.querySelector(".research-carousel-track");
    const slides = Array.from(carousel.querySelectorAll(".research-carousel-slide"));
    const prevBtn = carousel.querySelector(".research-carousel-btn.prev");
    const nextBtn = carousel.querySelector(".research-carousel-btn.next");
    const dotsContainer = document.getElementById("researchCarouselDots");

    if (!track || slides.length === 0 || !prevBtn || !nextBtn || !dotsContainer) return;

    /*
     * 五秒切换一次。
     * 注意：这是每张图的停留节奏，不是动画时间。
     * 动画时间由 CSS 中的 1050ms 控制。
     */
    const AUTOPLAY_DELAY = 5000;
    const TRANSITION_DURATION = 1050;

    let currentIndex = 0;
    let autoplayTimer = null;
    let isPaused = false;
    let isDestroyed = false;
    let isAnimating = false;

    const prefersReducedMotion =
      window.matchMedia &&
      window.matchMedia("(prefers-reduced-motion: reduce)").matches;

    const canAutoplay = slides.length > 1 && !prefersReducedMotion;
    const removeListeners = [];

    function addListener(element, eventName, handler) {
      element.addEventListener(eventName, handler, false);
      removeListeners.push(function () {
        element.removeEventListener(eventName, handler, false);
      });
    }

    dotsContainer.innerHTML = "";

    slides.forEach(function (_, index) {
      const dot = document.createElement("button");
      dot.className = "research-carousel-dot";
      dot.type = "button";
      dot.setAttribute("aria-label", "Go to slide " + (index + 1));

      addListener(dot, "click", function () {
        goToSlide(index);
        scheduleAutoplay();
      });

      dotsContainer.appendChild(dot);
    });

    const dots = Array.from(dotsContainer.querySelectorAll(".research-carousel-dot"));

    function clearAutoplay() {
      if (autoplayTimer !== null) {
        window.clearTimeout(autoplayTimer);
        autoplayTimer = null;
      }
    }

    function scheduleAutoplay() {
      clearAutoplay();

      if (isDestroyed || !canAutoplay || isPaused || document.hidden) {
        return;
      }

      autoplayTimer = window.setTimeout(function () {
        nextSlide();
        scheduleAutoplay();
      }, AUTOPLAY_DELAY);
    }

    function pauseAutoplay() {
      isPaused = true;
      clearAutoplay();
    }

    function resumeAutoplay() {
      isPaused = false;
      scheduleAutoplay();
    }

    function updateCarousel() {
      track.style.transform = "translate3d(-" + currentIndex * 100 + "%, 0, 0)";

      slides.forEach(function (slide, index) {
        slide.classList.toggle("active", index === currentIndex);
      });

      dots.forEach(function (dot, index) {
        dot.classList.toggle("active", index === currentIndex);
      });
    }

    function goToSlide(index) {
      if (slides.length <= 1) return;

      const nextIndex = (index + slides.length) % slides.length;

      if (nextIndex === currentIndex || isAnimating) {
        return;
      }

      currentIndex = nextIndex;
      isAnimating = true;
      updateCarousel();

      window.setTimeout(function () {
        isAnimating = false;
      }, TRANSITION_DURATION + 80);
    }

    function nextSlide() {
      goToSlide(currentIndex + 1);
    }

    function prevSlide() {
      goToSlide(currentIndex - 1);
    }

    addListener(nextBtn, "click", function () {
      nextSlide();
      scheduleAutoplay();
    });

    addListener(prevBtn, "click", function () {
      prevSlide();
      scheduleAutoplay();
    });

    /*
     * 鼠标悬停暂停，离开后恢复。
     * pointerenter / pointerleave 对 Mac Safari、Chrome、Edge 更稳。
     * mouseenter / mouseleave 作为补充兼容。
     */
    addListener(wrapper, "pointerenter", pauseAutoplay);
    addListener(wrapper, "pointerleave", resumeAutoplay);
    addListener(wrapper, "mouseenter", pauseAutoplay);
    addListener(wrapper, "mouseleave", resumeAutoplay);

    /*
     * 用户使用键盘或按钮聚焦时暂停，提高可访问性。
     */
    addListener(wrapper, "focusin", pauseAutoplay);
    addListener(wrapper, "focusout", resumeAutoplay);

    /*
     * 页面切到后台时暂停，回到前台后恢复。
     * 可以避免浏览器后台节流导致恢复时动画异常。
     */
    addListener(document, "visibilitychange", function () {
      if (document.hidden) {
        clearAutoplay();
      } else {
        scheduleAutoplay();
      }
    });

    /*
     * 支持左右键切换。
     */
    addListener(wrapper, "keydown", function (event) {
      if (event.key === "ArrowLeft") {
        prevSlide();
        scheduleAutoplay();
      }

      if (event.key === "ArrowRight") {
        nextSlide();
        scheduleAutoplay();
      }
    });

    if (!wrapper.hasAttribute("tabindex")) {
      wrapper.setAttribute("tabindex", "0");
    }

    /*
     * 初始化首张图的 active 状态。
     * 这样首张图片会有轻微的视觉进入效果，而不是静态显示。
     */
    updateCarousel();
    scheduleAutoplay();

    carousel.__researchCarouselInstance = {
      destroy: function () {
        isDestroyed = true;
        clearAutoplay();
        removeListeners.forEach(function (remove) {
          remove();
        });
        dotsContainer.innerHTML = "";
      }
    };
  }

  if (document.readyState === "loading") {
    document.addEventListener("DOMContentLoaded", initResearchCarousel, { once: true });
  } else {
    initResearchCarousel();
  }
})();
</script>

# BIO

I am now a lecturer at the School of Computer Science and Technology and the Hubei Provincial Key Laboratory of Intelligent Information Processing and Real-time Industrial Systems, Wuhan University of Science and Technology, Wuhan, China. I have received the B.S. degree in information security from the Wuhan University of Science and Technology, Wuhan, China, in 2017, and the Ph.D. degree in control science and engineering from Wuhan University of Science and Technology, Wuhan, China, in 2022. I was supervised by Professor `Kai Zhang`, who is the `Dean of the Graduate School of Wuhan University of Science and Technology`, the `Dean of the School of Computer Science and Technology at Wuhan University of Science and Technology`, the `Director of the Hubei Provincial Key Laboratory of Intelligent Information Processing and Real-time Industrial Systems` in China. From March to September 2025, I visited the School of Artificial Intelligence and Automation at Huazhong University of Science and Technology as a visiting scholar, under the guidance of Professor `Linqiang Pan`.

I am a member of the **Institute of Electrical and Electronics Engineers (IEEE)**, **China Computer Federation (CCF)**, **Association for Computing Machinery (ACM)**, **Chinese Association for Artificial Intelligence (CAAI)**, **Chinese Association of Automation (CAA)**, **Chinese Institute of Electronics (CIE)**, **IEEE Systems, Man, and Cybernetics Society (IEEE-SMC)**, **IEEE Computational Intelligence Society (IEEE-CIS)**, **Technical Committee on Intelligent Simulation Optimization and Scheduling, China Simulation Federation (CSF)** , and **ACM Special Interest Group on Genetic and Evolutionary Computation (ACM-SIGEVO)**. Recognized as a high-quality content creator and blogging expert in the field of artificial intelligence on CSDN, I have actively contributed to the academic community.

I was awarded the National Scholarship for Master's students in 2019 and the National Scholarship for Doctoral students in 2021 and 2022 by the Ministry of Education of China. Recently, I have achieved significant advancements and breakthroughs in multi-task multi-objective optimization, constrained multi-objective optimization, and many-objective optimization.

I have participated in two projects funded by the National Natural Science Foundation of China and led a youth project funded by the Provincial Natural Science Foundation. My research findings have been published in top-tier international journals such as **IEEE Transactions on Evolutionary Computation**, **IEEE Transactions on Cybernetics**, **IEEE Transactions on Intelligent Transportation Systems**, **Information Sciences**, **Science China: Information Sciences**, and **Applied Soft Computing**.

I was recognized as an Excellent Graduate Student at the Annual Meeting and Academic Seminar of the Wuhan Computer Software Engineering Society in both 2021 and 2022, and won the First Prize at the 2021 CCF Wuhan Excellent Doctoral Student Academic Showcase Forum. 

I serve as a reviewer for leading international journals including **IEEE Transactions on Evolutionary Computation**, **IEEE Transactions on Systems, Man, and Cybernetics: Systems**, **IEEE Transactions on Cybernetics**, **Information Sciences**, **Applied Soft Computing**, **Robotics and Computer-Integrated Manufacturing**, **Neural Computing and Applications**, **Engineering Applications of Artificial Intelligence**, **Expert Systems with Applications**, and **Journal of Membrane Computing**.

Additionally, I am a reviewer for international conferences such as the **IEEE Congress on Evolutionary Computation (IEEE CEC)**, **IEEE Symposium Series on Computational Intelligence (SSCI)**, **IEEE Conference on Artificial Intelligence (IEEE CAI)** and the **International Conference on Bio-inspired Computing: Theories and Applications (BIC-TA)**.

I have Served as a Session Chair at the **19th International Conference on Bio-inspired Computing: Theories and Applications (BIC-TA 2024)**, **20th International Conference on Bio-inspired Computing: Theories and Applications (BIC-TA 2025)**, Program Committee Member for the **2025 Asia Conference on Artificial Intelligence Technology (ACAIT2025)** and **The International Conference on Machine Intelligence and Nature-inspired Computing (MIND 2025)**.

My research interests include:

- Neural Combinatorial Optimization
- Scheduling and Vehicle Routing Planning
- Evolutionary Computation
- Multi-objective Optimization (Many-objective, Constrained, Multi-task, Multimodal, etc.)
- DNA Computing, Encoding, and Self-Assembly

## 📎 Homepages
- Personal Pages: https://JaywayXu.github.io (updated recently🔥)
- 中文站点：https://JaywayXu.github.io/zh-cn/ （`如果您是国内的学者，想要更多了解我们课题组的动态`）
- Google Scholar: https://scholar.google.com/citations?user=_Lkioz8AAAAJ&hl
- Researchgate: https://www.researchgate.net/profile/Zhiwei-Xu-16
- 微信公众号： 演化计算与人工智能
<img src="images/Wechat.png" alt="微信公众号" style="width: 300px; height: auto;">
- CSDN: 武科大许志伟 : https://xuzhiwei.blog.csdn.net/
<br>
- Email: xuzhiwei@wust.edu.cn

## 💻 Selected Research Papers
My full paper list is shown at [my personal homepage](https://JaywayXu.github.io/) or [中文主站](https://JaywayXu.github.io/zh-cn/).

---

## 💻 Selected Research Papers
My full paper list is shown at [my personal homepage](https://JaywayXu.github.io/) or [中文主站](https://JaywayXu.github.io/zh-cn/).

---
- `Zhiwei Xu(许志伟)` \*, Kai Zhang, Javier Del Ser, Miqing Li, Xin Xu, Juanjuan He, Ni Wu.Multi-Objective Optimization for Multimodal Multi-Objective Multi-Point Shortest Path Problem Considering Unforeseeable Road Eventualities. *IEEE Transactions on Intelligent Transportation Systems* , vol. 26, no. 6, pp. 8622-8640, June 2025. (JCR: Q1; IF: 7.9)  
[[Link]](https://ieeexplore.ieee.org/document/10959009/) [[Download]](https://jaywayxu.github.io/PDF/MMOEA-CDP.pdf) [[Code]](https://github.com/JaywayXu/MMOEA-CDP)

- Kai Zhang, `Zhiwei Xu(许志伟)`, Shengli Xie, and Gary G. Yen\*. Evolution Strategy-Based Many-Objective Evolutionary Algorithm Through Vector Equilibrium. *IEEE Transactions on Cybernetics* , vol. 51, no. 11, pp. 5455–5467, Nov. 2021. (JCR:Q1; IF:11.8)  
[[Link]](https://ieeexplore.ieee.org/document/8955947/) [[Download]](https://jaywayxu.github.io/PDF/MaOES.pdf)[[Code]](https://github.com/MaOEA/MaOES)

- Kai Zhang, `Zhiwei Xu(许志伟)`, Gary G. Yen\*, Ling Zhang. Two-Stage Multi-Objective Evolution Strategy for Constrained Multi-Objective Optimization. *IEEE Transactions on Evolutionary Computation* , vol. 28, no. 1, pp. 17–31, Feb. 2024 (JCR:Q1; IF:14.3)  
[[Link]](https://ieeexplore.ieee.org/document/9869698) [[Download]](https://jaywayxu.github.io/PDF/CMOES.pdf)[[Code]](https://github.com/MaOEA/CMOES)

- `Zhiwei Xu (许志伟)`, Xiaoming Liu, Kai Zhang\*, and Juanjuan He. Cultural transmission based multi-objective evolution strategy for evolutionary multitasking. *Information Sciences* , vol. 582, pp. 215–242, Jan. 2022. (JCR:Q1; IF：8.1)  
[[Link]](https://www.sciencedirect.com/science/article/pii/S0020025521009282) [[Download]](https://jaywayxu.github.io/PDF/CT_EMT_MOES.pdf)[[Code]](https://github.com/Asurada2015/CT-EMT-MOES)

- `Zhiwei Xu (许志伟)`, Kai Zhang, Juanjuan He\*, and Xiaoming Liu. A novel membrane-inspired evolutionary framework for multi-objective multi-task optimization problems. *Information Sciences* , vol. 596, pp. 236–263, Jun. 2022. (JCR:Q1; IF：8.1)  
[[Link]](https://www.sciencedirect.com/science/article/pii/S002002552200216X) [[Download]](https://jaywayxu.github.io/PDF/EMT-MOMIEA.pdf)

- `Zhiwei Xu (许志伟)` and Kai Zhang\*. Multiobjective multifactorial immune algorithm for multiobjective multitask optimization problems. *Applied Soft Computing* , vol. 107, p. 107399, Aug. 2021. (JCR:Q1; IF：8.7)  
[[Link]](https://www.sciencedirect.com/science/article/pii/S1568494621003227) [[Download]](https://jaywayxu.github.io/PDF/MOMFIA.pdf)

- `Zhiwei Xu (许志伟)`\*, Jia feng Xu, Kai Zhang, Xin Xu, Juanjuan He, Ni Wu, Decision Variable Classification based Multi-objective Multifactorial Memetic Algorithm for Multi-objective Multi-task Optimization Problem. *Applied Soft Computing* , vol. 152, p. 111232, Feb. 2024. (JCR:Q1; IF：8.7)  
[[Link]](https://www.sciencedirect.com/science/article/pii/S1568494624000061) [[Download]](https://jaywayxu.github.io/PDF/HMOMFMA.pdf)

