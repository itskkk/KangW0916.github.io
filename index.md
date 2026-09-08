---
layout: page
---

# About Me

<img src="{{ '/images/personal-photo.jpg' | relative_url }}" class="floatpic">

Here is **Chris Wang (王康)**.<br>

I am a PhD student in the [Department of Modern Mechanics](https://ses.ustc.edu.cn/) at the **University of Science and Technology of China**. Currently, I am studying and researching in the *Computational Mechanics and Engineering Laboratory (CME)* under the guidance of *[Professor Yinbo Zhu](https://scholar.google.com.hk/citations?hl=zh-CN&user=0IIXHuMAAAAJ)* and *[Professor Hengan Wu](https://scholar.google.com.hk/citations?hl=zh-CN&user=X4lTQbMAAAAJ)*. My research focuses on the design and nano-mechanics of amorphous carbon, with an emphasis on material structure design and computational materials science.<br>

## Education Experience

<div class="timeline">
  <div class="timeline-progress" id="timeline-progress"></div>

  <div class="timeline-item timeline-item--current timeline-item--ustc">
    <div class="timeline-dot" style="background: #ffffff;">
      <img src="{{ '/images/logo/ustc-emblem.jpg' | relative_url }}" alt="University of Science and Technology of China">
    </div>
    <div class="timeline-card">
      <div class="timeline-header">
        <div class="timeline-role">PhD Student <span class="timeline-sep">|</span> <span class="timeline-company">University of Science and Technology of China</span></div>
        <span class="timeline-time">Sep. 2024 - Present</span>
      </div>
      <div class="timeline-details">
        Department of Modern Mechanics. Supervised by <a href="https://scholar.google.com.hk/citations?hl=zh-CN&user=0IIXHuMAAAAJ">Prof. Yinbo Zhu</a> and <a href="https://scholar.google.com.hk/citations?hl=zh-CN&user=X4lTQbMAAAAJ">Prof. Hengan Wu</a>.
      </div>
    </div>
  </div>

  <div class="timeline-item timeline-item--hunan">
    <div class="timeline-dot" style="background: #ffffff;">
      <img src="{{ '/images/logo/hunan-emblem.jpg' | relative_url }}" alt="Hunan University">
    </div>
    <div class="timeline-card">
      <div class="timeline-header">
        <div class="timeline-role">BEng Student <span class="timeline-sep">|</span> <span class="timeline-company">Hunan University</span></div>
        <span class="timeline-time">Sep. 2020 - Jun. 2024</span>
      </div>
      <div class="timeline-details">
        Department of Engineering Mechanics. Supervised by <em>Prof. Yiru Ren</em>.
      </div>
    </div>
  </div>

</div>

<script>
(function() {
  var timelineProgress = document.getElementById('timeline-progress');
  var timeline = document.querySelector('.timeline');
  if (!timelineProgress || !timeline) return;

  var items = timeline.querySelectorAll('.timeline-item');

  // IntersectionObserver for in-view class
  if ('IntersectionObserver' in window) {
    var observer = new IntersectionObserver(function(entries) {
      entries.forEach(function(entry) {
        if (entry.isIntersecting) {
          entry.target.classList.add('in-view');
        }
      });
    }, { rootMargin: '0px 0px -15% 0px' });

    items.forEach(function(item, idx) {
      if (idx < 3) {
        // Reveal first 3 immediately on load (still gets the stagger transition)
        item.classList.add('in-view');
      } else {
        observer.observe(item);
      }
    });
  } else {
    items.forEach(function(item) { item.classList.add('in-view'); });
  }

  // Scroll progress bar
  window.addEventListener('scroll', function() {
    var rect = timeline.getBoundingClientRect();
    var totalHeight = timeline.offsetHeight;
    var windowH = window.innerHeight;
    var lineTop = 30;
    var lineBottom = 30;
    var lineHeight = totalHeight - lineTop - lineBottom;

    if (rect.top < windowH && rect.bottom > 0) {
      var scrolled = Math.min(1, Math.max(0, (windowH - rect.top - lineTop) / (totalHeight - lineTop + windowH * 0.4)));
      timelineProgress.style.height = Math.min(scrolled * lineHeight, lineHeight) + 'px';
    }
  }, { passive: true });
})();
</script>

---

## Publications

<div class="publications-grid">

  <div class="publication-card">
    <div class="publication-thumb">
      <img src="{{ '/images/papers/acsml.png' | relative_url }}" alt="Mechanical Amorphization-Mediated Self-Healing of Fractured Diamond">
      <a href="https://doi.org/10.1021/acsmaterialslett.5c01275" class="publication-overlay" target="_blank" rel="noopener">
        <span>View Paper</span>
      </a>
    </div>
    <div class="publication-info">
      <div class="publication-title">
        <a href="https://doi.org/10.1021/acsmaterialslett.5c01275" target="_blank" rel="noopener">Mechanical Amorphization-Mediated Self-Healing of Fractured Diamond</a>
      </div>
      <div class="publication-authors"><strong class="author-highlight">Kang Wang</strong>, HengAn Wu, YinBo Zhu</div>
      <div class="publication-conference"><span class="pub-venue">ACS Materials Letters, October 2025</span></div>
      <div class="publication-details">JCR Q1, IF = 8.7</div>
    </div>
  </div>

  <div class="publication-card">
    <div class="publication-thumb">
      <img src="{{ '/images/papers/acsnano.png' | relative_url }}" alt="Transformation-Mediated Kinetic Unfreezing in Mixed-Motif Amorphous Carbon">
      <a href="https://doi.org/10.1021/acsnano.6c10835" class="publication-overlay" target="_blank" rel="noopener">
        <span>View Paper</span>
      </a>
    </div>
    <div class="publication-info">
      <div class="publication-title">
        <a href="https://doi.org/10.1021/acsnano.6c10835" target="_blank" rel="noopener">Transformation-Mediated Kinetic Unfreezing in Mixed-Motif Amorphous Carbon</a>
      </div>
      <div class="publication-authors"><strong class="author-highlight">Kang Wang</strong>, ZhongTing Zhang, HengAn Wu, YinBo Zhu</div>
      <div class="publication-conference"><span class="pub-venue">ACS Nano, July 2026</span></div>
      <div class="publication-details">JCR Q1, IF = 16.1</div>
    </div>
  </div>

  <div class="publication-card">
    <div class="publication-thumb">
      <img src="{{ '/images/papers/ijcr.jpg' | relative_url }}" alt="Energy absorption performance of multi-cell hexagonal tube with hierarchical self-similarity">
      <a href="https://doi.org/10.1080/13588265.2026.2716950" class="publication-overlay" target="_blank" rel="noopener">
        <span>View Paper</span>
      </a>
    </div>
    <div class="publication-info">
      <div class="publication-title">
        <a href="https://doi.org/10.1080/13588265.2026.2716950" target="_blank" rel="noopener">Energy absorption performance of multi-cell hexagonal tube with hierarchical self-similarity</a>
      </div>
      <div class="publication-authors"><strong class="author-highlight">Kang Wang</strong>, YiRu Ren</div>
      <div class="publication-conference"><span class="pub-venue">International Journal of Crashworthiness, August 2026</span></div>
      <div class="publication-details">JCR Q3, IF = 1.8</div>
    </div>
  </div>

</div>

<script>
(function() {
  if ('IntersectionObserver' in window) {
    var observer = new IntersectionObserver(function(entries) {
      entries.forEach(function(entry) {
        if (entry.isIntersecting) {
          entry.target.classList.add('animate-in');
          observer.unobserve(entry.target);
        }
      });
    }, { threshold: 0.08, rootMargin: '0px 0px -40px 0px' });
    document.querySelectorAll('.publication-card').forEach(function(card) {
      observer.observe(card);
    });
  } else {
    document.querySelectorAll('.publication-card').forEach(function(card) {
      card.classList.add('animate-in');
    });
  }
})();
</script>

---

## Research Interests

- Nano Mechanics of Amorphous Carbon
- Material Structure Design
- Computational Materials Science

My research focuses on the relationship between the structure and mechanical behavior of amorphous carbon, using computational materials science and atomistic simulation to explore material structure design and nano-mechanical mechanisms.

---

## News and Updates

<div class="news-grid">
  <div class="news-card news-card--milestone">
    <div class="news-meta">
      <span class="news-date">September 2026</span>
      <span class="news-tag news-tag--milestone">Milestone</span>
    </div>
    <p>Received PhD offer from the University of Science and Technology of China.</p>
  </div>

  <div class="news-card news-card--publication">
    <div class="news-meta">
      <span class="news-date">August 2026</span>
      <span class="news-tag news-tag--publication">Publication</span>
    </div>
    <p><strong>Energy absorption performance of multi-cell hexagonal tube with hierarchical self-similarity</strong> published in <em>International Journal of Crashworthiness</em> (JCR IF=1.8).</p>
  </div>

  <div class="news-card news-card--publication">
    <div class="news-meta">
      <span class="news-date">July 2026</span>
      <span class="news-tag news-tag--publication">Publication</span>
    </div>
    <p><strong>Transformation-Mediated Kinetic Unfreezing in Mixed-Motif Amorphous Carbon</strong> published in <em>ACS Nano</em> (JCR IF=16.1).</p>
  </div>

  <div class="news-card news-card--publication">
    <div class="news-meta">
      <span class="news-date">October 2025</span>
      <span class="news-tag news-tag--publication">Publication</span>
    </div>
    <p><strong>Mechanical Amorphization-Mediated Self-Healing of Fractured Diamond</strong> published in <em>ACS Materials Letters</em> (JCR IF=8.7).</p>
  </div>

  <div class="news-card news-card--milestone">
    <div class="news-meta">
      <span class="news-date">September 2024</span>
      <span class="news-tag news-tag--milestone">Milestone</span>
    </div>
    <p>Join to CME Lab, University of Science and Technology of China.</p>
  </div>
</div>

<script>
(function() {
  if ('IntersectionObserver' in window) {
    var observer = new IntersectionObserver(function(entries) {
      entries.forEach(function(entry) {
        if (entry.isIntersecting) {
          entry.target.classList.add('animate-in');
          observer.unobserve(entry.target);
        }
      });
    }, { threshold: 0.08, rootMargin: '0px 0px -60px 0px' });
    document.querySelectorAll('.news-card').forEach(function(card) {
      observer.observe(card);
    });
  } else {
    document.querySelectorAll('.news-card').forEach(function(card) {
      card.classList.add('animate-in');
    });
  }
})();
</script>
