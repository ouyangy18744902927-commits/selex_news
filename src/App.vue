<script setup>
const registrationUrl =
  "https://aptamers.feishu.cn/share/base/form/shrcny8IdUtO08t3y9wNmDa3Pnb";
const email = "aptamer@him.cas.cn";

const sections = [
  {
    title: "开场导语",
    type: "intro",
    paragraphs: [
      "核酸适体（Aptamer）在分子诊断、传感检测、药物递送、靶向治疗、蛋白质组学等领域应用前景广阔。",
      "但在真实研究与转化过程中，行业仍面临筛选门槛高、验证标准不统一、数据分散、应用转化不足等问题。",
      "7月15日-17日，中国科学院杭州医学研究所核酸适体筛选中心将举办第四届免费直播大会，并全面升级为“实战体验营”。",
    ],
  },
  {
    title: "本次体验营看什么",
    type: "bullets",
    items: [
      "三天时间，真实跑通两轮完整 SELEX 筛选流程。",
      "从靶标到验证，全流程直播展示。",
      "关键技术环节边做边讲，现场拆解实验思路。",
      "直播期间实时答疑，帮助参会者理解从筛选到应用的关键节点。",
    ],
  },
  {
    title: "平台与技术支撑",
    type: "text",
    paragraphs: [
      "本次直播培训依托中国科学院杭州医学研究所核酸适体筛选中心及分子相互作用平台。平台面向蛋白、核酸、药物分子等多类型生物分子，围绕核酸适体筛选、分子互作分析、核酸检测定量和自动化流程开发，建立了从筛选到验证的技术支撑体系。",
      "平台可提供抗体筛选、药物筛选、亲和力测试、抗体结合表位测试、核酸适体筛选，以及自动化工作流程开发等服务，为科研合作和应用转化提供支撑。",
    ],
    image: {
      src: "/assets/platform.jpg",
      alt: "分子相互作用平台实验环境，可支撑核酸适体筛选、分子互作分析和样本检测等工作。",
      caption: "图注：分子相互作用平台实验环境，可支撑核酸适体筛选、分子互作分析和样本检测等工作。",
    },
  },
  {
    title: "主要仪器",
    type: "gallery",
    paragraphs: [
      "平台配置覆盖筛选、定量、互作验证和样本分析的关键设备，包括 SPR、ITC、BLI、数字 PCR、荧光定量 PCR、核酸片段分析、生物制药分析和单细胞分离等系统。",
      "这些设备共同支撑核酸适体研究中的样本制备、轮次监测、亲和力评价、结合验证和质量控制。",
    ],
    images: [
      {
        src: "/assets/spr.jpg",
        alt: "表面等离子共振分子互作系统：用于实时检测分子结合过程和亲和力参数。",
        caption: "图注：表面等离子共振分子互作系统：用于实时检测分子结合过程和亲和力参数。",
      },
      {
        src: "/assets/itc.jpg",
        alt: "等温滴定微量热仪：用于无标记测定分子结合热力学参数。",
        caption: "图注：等温滴定微量热仪：用于无标记测定分子结合热力学参数。",
      },
      {
        src: "/assets/bli.jpg",
        alt: "生物膜干涉分子互作系统：适合多样本亲和力测试和抗体/适体结合验证。",
        caption: "图注：生物膜干涉分子互作系统：适合多样本亲和力测试和抗体/适体结合验证。",
      },
      {
        src: "/assets/detection_group.jpg",
        alt: "数字 PCR、荧光定量 PCR 与核酸片段分析等设备：用于筛选轮次样本检测、扩增监测、绝对定量和片段质量控制。",
        caption: "图注：数字 PCR、荧光定量 PCR 与核酸片段分析等设备：用于筛选轮次样本检测、扩增监测、绝对定量和片段质量控制。",
      },
    ],
  },
  {
    title: "专业实验室",
    type: "text",
    paragraphs: [
      "围绕 SELEX 筛选的实际流程，平台建设了分子互作实验室和核酸分析、检测、定量实验室。前者侧重结合过程与亲和力评价，后者侧重核酸模板检测、扩增监测和片段质量控制。",
      "两个实验室可以将筛选、扩增、定量、互作验证等步骤顺畅衔接，帮助研究者从“获得候选序列”进一步走向“确认可用分子”。",
    ],
    image: {
      src: "/assets/interaction_lab_group.jpg",
      alt: "分子互作实验室相关设备：支持候选分子的结合验证和亲和力评价。",
      caption: "图注：分子互作实验室相关设备：支持候选分子的结合验证和亲和力评价。",
    },
    secondaryImage: {
      src: "/assets/nucleic_lab_group.jpg",
      alt: "核酸分析、检测、定量相关设备：支撑筛选过程中的模板检测、片段质控和结果确认。",
      caption: "图注：核酸分析、检测、定量相关设备：支撑筛选过程中的模板检测、片段质控和结果确认。",
    },
  },
  {
    title: "核酸适体自动化筛选实验室",
    type: "text",
    paragraphs: [
      "核酸适体自动化筛选实验室已开发多代自动化仪器。",
      "第一代为半自动化筛选仪，可实现多靶标平行筛选；第二代自动化筛选工作站可实现单轮自动化筛选，移液、孵育、PCR、制备单链等操作均可自动化运行；第三代自动化工作站进一步集成酶标仪、撕膜机、封膜机、离心机、核酸片段分析仪、工作站和 PCR 仪，形成全自动化核酸适体筛选系统。",
      "实验室既可以提供筛选服务，也可以提供自动化流程开发服务。",
    ],
    image: {
      src: "/assets/auto_workstation.jpg",
      alt: "核酸适体自动化筛选工作站：自动化工作站可提高筛选流程稳定性，减少人工操作差异。",
      caption: "图注：核酸适体自动化筛选工作站：自动化工作站可提高筛选流程稳定性，减少人工操作差异。",
    },
    secondaryImage: {
      src: "/assets/auto_modules.jpg",
      alt: "全自动化核酸适体筛选系统及配套模块：多模块集成，支撑筛选、孵育、扩增、制备单链和检测分析等流程衔接。",
      caption: "图注：全自动化核酸适体筛选系统及配套模块：多模块集成，支撑筛选、孵育、扩增、制备单链和检测分析等流程衔接。",
    },
  },
  {
    title: "超高通量分子互作分析平台",
    type: "text",
    paragraphs: [
      "团队自主研制核酸-蛋白高通量测序与互作一体化分析平台，面向大规模基因型-表型数据获取，突破传统互作分析方式在成本和通量方面的限制。",
      "该平台可在高通量测序仪底座上，通过微流控液路与光学探测系统改造，实现百万至千万级核酸分子与靶标蛋白的并行互作检测。",
    ],
    image: {
      src: "/assets/linx.jpg",
      alt: "自主研制的超高通量分子相互作用分析仪：面向百万至千万级核酸分子与靶标蛋白并行互作检测，为大规模筛选和数据获取提供支撑。",
      caption: "图注：自主研制的超高通量分子相互作用分析仪：面向百万至千万级核酸分子与靶标蛋白并行互作检测，为大规模筛选和数据获取提供支撑。",
    },
  },
];

const schedule = [
  "时间：2026年7月15日-17日（每天 9:00-12:00，14:00-17:00）",
  "形式：线上直播（免费）+ 线下限量席位",
  "主办：中国科学院杭州医学研究所 核酸适体筛选中心",
];

const timeline = [
  "7月15日上午：生态建设发布会，中心资源与合作机制介绍，合作伙伴成果分享。",
  "7月15日下午-17日：两轮 SELEX 筛选全流程直播培训 + 实时答疑。",
];

const audience = [
  "有蛋白 / 小分子 / 细胞 / 疾病靶标，想开展 aptamer 合作研究。",
  "从事分子诊断、传感检测、POCT、外泌体、蛋白质组学、药物递送等方向。",
  "拥有临床样本或真实应用场景，希望推进技术转化。",
  "想系统了解从筛选到应用的完整流程。",
  "希望与中心建立长期合作。",
];
</script>

<template>
  <main class="page">
    <header class="hero">
      <div class="eyebrow">第四届核酸适体筛选免费直播大会 · 合作生态建设发布会</div>
      <h1>SELEX技术直播培训与实战体验营</h1>
      <p class="meta">2026年7月15日-17日</p>
      <p class="submeta">三天实战直播，两轮完整 SELEX 流程，从靶标到验证，边做边讲，实时答疑。</p>
      <div class="actions">
        <a class="btn btn-primary" :href="registrationUrl" target="_blank" rel="noopener">报名链接</a>
        <a class="btn btn-secondary" :href="'mailto:' + email">咨询邮箱</a>
      </div>
      <div class="lead">
        把“适体筛选”做成可以看懂、可以转发、可以落地的网页版本，适合公众号发布与手机浏览。
      </div>
    </header>

    <section class="content">
      <article class="panel" v-for="section in sections" :key="section.title">
        <div class="panel-header">
          <h2>{{ section.title }}</h2>
        </div>
        <div class="panel-body">
          <template v-if="section.type === 'intro' || section.type === 'text'">
            <div class="intro">
              <p v-for="(paragraph, index) in section.paragraphs" :key="index">{{ paragraph }}</p>
            </div>
          </template>

          <template v-if="section.type === 'bullets'">
            <div class="bullets">
              <div class="bullet" v-for="item in section.items" :key="item">{{ item }}</div>
            </div>
          </template>

          <template v-if="section.type === 'text' || section.type === 'gallery'">
            <p v-for="(paragraph, index) in section.paragraphs" :key="index + '_p'">{{ paragraph }}</p>
          </template>

          <figure v-if="section.image" class="figure">
            <img :src="section.image.src" :alt="section.image.alt" loading="lazy" />
            <figcaption class="caption">{{ section.image.caption }}</figcaption>
          </figure>

          <figure v-if="section.secondaryImage" class="figure">
            <img :src="section.secondaryImage.src" :alt="section.secondaryImage.alt" loading="lazy" />
            <figcaption class="caption">{{ section.secondaryImage.caption }}</figcaption>
          </figure>

          <div v-if="section.images" class="gallery">
            <figure v-for="image in section.images" :key="image.src">
              <img :src="image.src" :alt="image.alt" loading="lazy" />
              <figcaption class="caption">{{ image.caption }}</figcaption>
            </figure>
          </div>
        </div>
      </article>

      <article class="panel">
        <div class="panel-header">
          <h2>会议信息</h2>
        </div>
        <div class="panel-body">
          <div class="info-grid">
            <div class="info" v-for="item in schedule" :key="item">{{ item }}</div>
          </div>
        </div>
      </article>

      <article class="panel">
        <div class="panel-header">
          <h2>日程概览</h2>
        </div>
        <div class="panel-body">
          <div class="info-grid">
            <div class="info" v-for="item in timeline" :key="item">{{ item }}</div>
          </div>
        </div>
      </article>

      <article class="panel">
        <div class="panel-header">
          <h2>适合谁参加？</h2>
        </div>
        <div class="panel-body">
          <div class="bullets">
            <div class="bullet" v-for="item in audience" :key="item">{{ item }}</div>
          </div>
        </div>
      </article>

      <article class="panel">
        <div class="panel-header">
          <h2>参会福利</h2>
        </div>
        <div class="panel-body">
          <div class="info">报名即送 2024 年培训完整剪辑视频（双语字幕）。</div>
        </div>
      </article>

      <article class="panel">
        <div class="panel-header">
          <h2>报名方式</h2>
        </div>
        <div class="panel-body">
          <div class="info-grid">
            <div class="info">
              报名链接：
              <a :href="registrationUrl" target="_blank" rel="noopener">{{ registrationUrl }}</a>
            </div>
            <div class="info">
              咨询邮箱：
              <a :href="'mailto:' + email">{{ email }}</a>
            </div>
          </div>
        </div>
      </article>

      <footer class="footer">
        <div class="ending">7月15日，线上见！</div>
        <div class="org">中科院杭州医学所 核酸适体筛选中心</div>
      </footer>
    </section>
  </main>
</template>
