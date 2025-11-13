---
layout: archive
title: "People/团队成员"
permalink: /people/
author_profile: true
---

{% include base_path %}

<style>
.people-container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 16px;
  box-sizing: border-box;
}

/* 教师区：左图右文 */
.teacher-section {
  display: flex;
  align-items: flex-start;
  gap: 24px;
  margin-bottom: 50px;
}
.teacher-photo {
  width: 220px;
  height: auto;
  object-fit: cover;
  border-radius: 0;
  box-shadow: 0 2px 8px rgba(0,0,0,0.1);
}
.teacher-info h2 { margin: 0 0 6px 0; }
.teacher-info p { 
  margin: 4px 0; 
  color: var(--text-color, #333); 
}
.teacher-info ul li {
  color: var(--text-color, #333);
}
html[data-theme="dark"] .teacher-info p,
html[data-theme="dark"] .teacher-info ul li {
  color: #ddd; /* 暗色模式下可读 */
}

/* 学生区：每行三人 */
.student-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 24px;
  margin-top: 16px;
}

/* 学生卡片 */
.student-card {
  display: flex;
  align-items: flex-start;
  gap: 14px;
  background: #fafafa;
  border-radius: 6px;
  box-shadow: 0 2px 6px rgba(0,0,0,0.05);
  padding: 10px;
  transition: transform 0.2s, box-shadow 0.2s;
}
.student-card:hover {
  transform: translateY(-4px);
  box-shadow: 0 4px 12px rgba(0,0,0,0.1);
}

.student-photo {
  width: 150px;
  height: 210px;
  object-fit: cover;
  border-radius: 0;
}
.student-info { flex: 1; }
.student-info p {
  margin: 0 0 6px 0;
  font-size: 15px;
  color: var(--text-color, #222);
  line-height: 1.4em;
}
.student-info strong { font-size: 16px; }

@media (max-width: 900px) {
  .student-grid { grid-template-columns: repeat(2, 1fr); }
  .teacher-section { flex-direction: column; align-items: center; text-align: center; }
}
@media (max-width: 600px) {
  .student-grid { grid-template-columns: 1fr; }
  .student-card { flex-direction: row; }
}

/* 只修改学生名字的超链接颜色 */
.student-link {
  text-decoration: none; /* 去除下划线 */
  color: #007bff; /* 修改为网站链接一致的颜色 */
}

/* 超链接悬停效果 */
.student-link:hover {
  text-decoration: underline; /* 悬停时显示下划线 */
  color: #0056b3; /* 悬停时的颜色变化 */
}

</style>

<div class="people-container">


<!-- ================= 教师 ================= -->
<section class="teacher-section">
  <img class="teacher-photo" src="/images/weitang_photo.png" alt="唐伟">
  <div class="teacher-info">
    <h2>唐 伟 <small>副教授 / 博导</small></h2>
    <h3>中国矿业大学（北京） 地球科学与测绘工程学院</h3>

    <h4>研究方向</h4>
    <ul>
      <li>空间大地测量技术（SAR / InSAR / GNSS）</li>
      <li>地表形变灾害监测与风险评估（地面沉降、滑坡、采动沉陷等）</li>
      <li>含水层地面沉降监测与地下水资源可持续管理</li>
      <li>地球物理建模与参数反演</li>
    </ul>
  </div>
</section>

<hr />

<!-- ================= 博士生 ================= -->
<h3>博士生</h3>
<div class="student-grid">
  <div class="student-card">
    <img class="student-photo" src="/files/students/liuying.jpg" alt="刘莹">
    <div class="student-info">
      <p><strong>刘莹</strong></p>
      <p><strong>博士 2025级</strong></p>
      <p>研究InSAR相位解缠误差改正算法。</p>
    </div>
  </div>

  <div class="student-card">
  <img class="student-photo" src="/files/students/lixuepeng.jpg" alt="李雪鹏">
  <div class="student-info">
    <p><strong>李雪鹏</strong></p>
    <p><strong>博士 2025级</strong></p>
    <p>
      研究方向为基于InSAR技术的华北平原地下水储量和水文参数研究。<br>
      ResearchGate：<a href="https://www.researchgate.net/profile/Xuepeng-Li-6?ev=prf_overview" target="_blank">Xuepeng Li</a>
    </p>
  </div>
</div>


  <div class="student-card">
    <img class="student-photo" src="/files/students/zhaoxiangjun.jpg" alt="赵祥君">
    <div class="student-info">
      <p><strong><a href="https://1ife1over.github.io/" target="_blank">赵祥君</a></strong></p>
      <p><strong>博士 2023级</strong></p>
      <p>研究含水层InSAR地面沉降监测与地下水资源可持续管理。</p>
    </div>
  </div>
</div>

<!-- ================= 硕士生 ================= -->
<h3>硕士生</h3>
<div class="student-grid">

  <div class="student-card">
    <img class="student-photo" src="/files/students/zhusijie.jpg" alt="朱斯杰">
    <div class="student-info">
      <p><strong>朱斯杰</strong></p>
      <p><strong>硕士 2025级</strong></p>
      <p>InSAR数据处理与多源数据融合。</p>
    </div>
  </div>

  <div class="student-card">
    <img class="student-photo" src="/files/students/liuxinrui.jpg" alt="刘莘瑞">
    <div class="student-info">
      <p><strong>刘莘瑞</strong></p>
      <p><strong>硕士 2025级</strong></p>
      <p>从事时间序列InSAR与地下水动态研究。</p>
    </div>
  </div>

  <div class="student-card">
    <img class="student-photo" src="/files/students/matengfei.jpg" alt="马腾飞">
    <div class="student-info">
      <p><strong>马腾飞</strong></p>
      <p><strong>硕士 2025级</strong></p>
      <p>来自河南省三门峡市，本科毕业于河南理工大学，喜欢打篮球，打羽毛球，性格外向。</p>
    </div>
  </div>

  <div class="student-card">
    <img class="student-photo" src="/files/students/zhaojingyu.jpg" alt="赵菁钰">
    <div class="student-info">
      <p><strong>赵菁钰</strong></p>
      <p><strong>硕士 2025级</strong></p>
      <p>山东德州人，本科毕业于山东科技大学，研究方向为新疆昌吉农业区地下水超采及地面沉降的监测与分析。</p>
    </div>
  </div>

  <div class="student-card">
    <img class="student-photo" src="/files/students/lijiawei.jpg" alt="李家炜">
    <div class="student-info">
      <p><strong>李家炜</strong></p>
      <p><strong>硕士 2025级</strong></p>
      <p>研一，男，24岁，山西朔州人。研究方向为InSAR地表沉降建模与趋势分析。性格开朗乐观，积极向上。</p>
    </div>
  </div>

  <div class="student-card">
    <img class="student-photo" src="/files/students/leiyiming.jpg" alt="雷一鸣">
    <div class="student-info">
      <p><strong>雷一鸣</strong></p>
      <p><strong>硕士 2024级</strong></p>
      <p>研究油气储层地面沉降反演与数值模拟。</p>
    </div>
  </div>

  <div class="student-card">
    <img class="student-photo" src="/files/students/zengling.jpg" alt="曾羚">
    <div class="student-info">
      <p><strong>曾羚</strong></p>
      <p><strong>硕士 2024级</strong></p>
      <p>北京市InSAR地面沉降/回弹机理与地下水位响应关系。</p>
    </div>
  </div>

  <div class="student-card">
    <img class="student-photo" src="/files/students/lixingchong.jpg" alt="李兴冲">
    <div class="student-info">
      <p><strong>李兴冲</strong></p>
      <p><strong>硕士 2024级</strong></p>
      <p>从事多时相InSAR技术在交通设施沉降监测中的应用及风险评估。</p>
    </div>
  </div>

  <div class="student-card">
    <img class="student-photo" src="/files/students/weixueting.jpg" alt="位雪婷">
    <div class="student-info">
      <p><strong>位雪婷</strong></p>
      <p><strong>硕士 2024级</strong></p>
      <p>研究苏锡常地区地面沉降与地下水水位变化关系。</p>
    </div>
  </div>

  <div class="student-card">
    <img class="student-photo" src="/files/students/liyonghui.jpg" alt="李兴冲">
    <div class="student-info">
      <p><strong>李永辉</strong></p>
      <p><strong>硕士 2023级</strong></p>
      <p>辽河三角洲海岸线地面沉降研究。</p>
    </div>
  </div>

  <div class="student-card">
    <img class="student-photo" src="/files/students/linchunyan.jpg" alt="林春燕">
    <div class="student-info">
      <p><strong>林春艳</strong></p>
      <p><strong>硕士 2023级</strong></p>
      <p>研究华北平原地面沉降机理，并结合地质、地下水、土地利用、降雨等影响因子模拟地面沉降。</p>
    </div>
  </div>

  <div class="student-card">
    <img class="student-photo" src="/files/students/wangyiming.jpg" alt="王一鸣">
    <div class="student-info">
      <p><strong>王一鸣</strong></p>
      <p><strong>硕士 2023级</strong></p>
      <p>太原市小店区InSAR地面沉降监测与地下水位变化耦合关系。</p>
    </div>
  </div>

  <div class="student-card">
    <img class="student-photo" src="/files/students/weizihan.jpg" alt="魏子涵">
    <div class="student-info">
      <p><strong>魏子涵</strong></p>
      <p><strong>硕士 2023级</strong></p>
      <p>关注地下水资源与环境影响。</p>
    </div>
  </div>

  <div class="student-card">
    <img class="student-photo" src="/files/students/chengshuaishuai.jpg" alt="成帅帅">
    <div class="student-info">
      <p><strong>成帅帅</strong></p>
      <p><strong>硕士 2023级</strong></p>
      <p>研究地表形变与气候变化关系。</p>
    </div>
  </div>

  <div class="student-card">
    <img class="student-photo" src="/files/students/liukai.jpg" alt="刘凯">
    <div class="student-info">
      <p><strong>刘凯</strong></p>
      <p><strong>硕士 2023级</strong></p>
      <p>河北衡水人，本科毕业于华北理工大学测绘工程专业，研究方向为InSAR矿山形变监测应用。。</p>
    </div>
  </div>

  <div class="student-card">
    <img class="student-photo" src="/files/students/fuyu.jpg" alt="付煜">
    <div class="student-info">
      <p><strong>付煜</strong></p>
      <p><strong>硕士 2022级</strong></p>
      <p>时间序列InSAR与GNSS测量地表形变、地下水位变化与地表形变关联分析。现就职于中国铁路设计集团。</p>
    </div>
  </div>

  <div class="student-card">
    <img class="student-photo" src="/files/students/gengxu.jpg" alt="耿旭">
    <div class="student-info">
      <p><strong>耿旭</strong></p>
      <p><strong>硕士 2022级</strong></p>
      <p>从事地震与地面沉降的关联研究。</p>
    </div>
  </div>

  <div class="student-card">
    <img class="student-photo" src="/files/students/changjilong.jpg" alt="常纪龙">
    <div class="student-info">
      <p><strong>常纪龙</strong></p>
      <p><strong>硕士 2022级</strong></p>
      <p>InSAR与GNSS融合处理。现就职于北京市测绘院，从事大地测量数据解算与应用研究，北京市CORS系统运维。</p>
    </div>
  </div>

  <div class="student-card">
    <img class="student-photo" src="/files/students/zhutongzuo.jpg" alt="朱桐作">
    <div class="student-info">
      <p><strong>朱桐作</strong></p>
      <p><strong>硕士 2022级</strong></p>
      <p>InsAR地面沉降建模与监测，现就职于重庆规划和自然资源调查监测院，从事自然资源和不动产权籍调查工作。</p>
    </div>
  </div>

  <div class="student-card">
    <img class="student-photo" src="/files/students/chengsiyu.jpg" alt="成思雨">
    <div class="student-info">
      <p><strong>成思雨</strong></p>
      <p><strong>硕士 2021级</strong></p>
      <p>研究汾河流域InSAR地面沉降-回弹机理。</p>
    </div>
  </div>

  <div class="student-card">
    <img class="student-photo" src="/files/students/hubaojun.jpg" alt="胡宝俊">
    <div class="student-info">
      <p><strong>胡宝俊</strong></p>
      <p><strong>硕士 2021级</strong></p>
      <p>研究InSAR矿山形变监测应用。</p>
    </div>
  </div>

  <div class="student-card">
    <img class="student-photo" src="/files/students/chengqing.jpg" alt="程清">
    <div class="student-info">
      <p><strong>程清</strong></p>
      <p><strong>硕士 2021级</strong></p>
      <p>研究InSAR洪水面提取。</p>
    </div>
  </div>

  <div class="student-card">
    <img class="student-photo" src="/files/students/wangjinyang.jpg" alt="赵祥君">
    <div class="student-info">
      <p><strong>赵祥君</strong></p>
      <p><strong>硕士 2020级</strong></p>
      <p>研究太原盆地地面沉降时序InSAR监测与季节性变形小波分析。</p>
    </div>
  </div>

  <div class="student-card">
    <img class="student-photo" src="/files/students/wangjinyang.jpg" alt="王金洋">
    <div class="student-info">
      <p><strong>王金洋</strong></p>
      <p><strong>硕士 2020级</strong></p>
      <p>地下水回升条件下太原市地面沉降时空演变特征研究。</p>
    </div>
  </div>

</div>

</div>






