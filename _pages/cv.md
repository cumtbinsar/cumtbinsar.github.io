---
layout: archive
title: "CV/简历"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
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

</style>


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


教育经历
======
* 访问学者  2024-12——2025-03 
  * 德国莱布尼茨-汉诺威大学访问学者（DAAD再次邀请奖学金）
* 博士后    2017-2018  
  * 德国地学研究中心GFZ（中德（CSC-DAAD）博士后奖学金资助）
* 博士      2013-2017  
  * 武汉大学测绘遥感信息工程国家重点实验室摄影测量与遥感专业 
* 硕士      2010-2013 
  * 武汉大学测绘遥感信息工程国家重点实验室摄影测量与遥感专业

工作经历
======
* 2024-- 中国矿业大学（北京）地球科学与测绘工程学院--博导
* 2021-2024 中国矿业大学（北京）地球科学与测绘工程学院--副教授
* 2017-2021 中国矿业大学（北京）地球科学与测绘工程学院--讲师
  
代表性科研项目
======
* 综合多源大地测量研究汾河流域地下水位回升对区域地面沉降的调控作用机制，国家自然科学基金（面上）项目，2024.01-2027.12，主持

* 科学传播类：地下水、地面沉降与联合国2030可持续发展目标，国家自然科学基金（科技活动）项目，2024.08-2025.12，主持

* 煤炭矿区森林地上碳储量及开采-复垦累积效应定量模型，国家重点研发计划 政府间合作项目专题，子课题，主持

* 辽河三角洲油田开采地面沉降InSAR监测项目，校地合作项目，主持

* 融合InSAR、GNSS观测和WRF模式反演高空间分辨率大气可降水量, 国家自然科学基金（青年）项目，2021.01-2023.12，主持

* 山西省煤矿智能化变革推动黄河流域生态提升战略研究，中国工程院咨询研究项目

* 基于InSAR研究京津冀平原地下水位回升对地面沉降的影响机制，水利部京津冀水安全保障重点实验室开放基金项目，主持

* 神东矿区多源异构变形监测数据整合模型与评价体系研究，国家重点实验室开放基金，主持

* 基于InSAR技术反演大气水汽总量的方法研究，武汉大学测绘遥感信息工程国家重点实验室开放基金项目，主持

* 神东矿区地表沉陷观测系统建立与采动裂缝特征研究，神华集团科技创新项目

* 高分遥感InSAR地质灾害识别项目，校地合作项目，主持

* 宁东煤炭基地采煤塌陷区地表变形雷达监测项目，校地合作项目，参与

* 辽宁省矿区地面沉陷及塌陷InSAR调查项目，校地合作项目，主持


代表性科研论文
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  

