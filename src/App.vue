<script setup>
const effectiveDate = '2025年9月24日'
const contactEmail = 'kefu@aifindjob.fun'
const contactAddress =
  '上海市浦东新区张江高科技园区碧波路635号3号楼1001室'

const sections = [
  {
    id: 'intro',
    title: null,
    paragraphs: [
      '选我AI Tech Co., Ltd.（以下简称"选我AI"或"我们"）重视您的隐私。本隐私政策（以下简称"本政策"）解释了我们如何收集、使用、披露、保护和处理您在使用 选我AI 平台、网站、移动应用程序及相关服务（以下简称"服务"）时提供的信息。',
      '本政策适用于所有使用服务的用户（以下简称"您"或"用户"）。在使用服务前，请仔细阅读本政策。如果您不同意本政策，请勿使用服务。您的使用即表示您同意我们按照本政策处理您的信息。',
      '我们可能会不时更新本政策，更新后将在服务中发布通知。继续使用服务即表示您接受更新。',
    ],
  },
  {
    id: 'collection',
    title: '1. 我们收集的信息',
    paragraphs: [
      '我们收集以下类型的信息，以提供和改进服务：',
    ],
    subsections: [
      {
        title: '1.1 您提供的信息',
        items: [
          '注册信息：电子邮件地址、手机号码、姓名、密码等。',
          '个人信息：简历、求职偏好、工作经验、教育背景、技能等。',
          '通信信息：您与我们或平台上其他用户的消息、反馈、评论。',
          '支付信息：如果使用付费服务，我们收集必要的支付细节（但不存储信用卡信息，由第三方支付处理器处理）。',
        ],
      },
      {
        title: '1.2 自动收集的信息',
        items: [
          '设备信息：IP 地址、浏览器类型、操作系统、设备标识符。',
          '使用信息：访问时间、页面浏览、点击行为、搜索查询。',
          '位置信息：如果您启用，我们可能收集大致位置数据。',
          'Cookie 和类似技术：我们使用 Cookie、像素标签等来分析使用模式、个性化内容和投放广告。详情见第 6 节。',
        ],
      },
      {
        title: '1.3 来自第三方的信息',
        items: [
          '如果您通过第三方账户（如微信、Google）登录，我们可能从这些服务获取基本信息。',
          '我们可能从合作伙伴或公开来源获取补充信息，以增强服务。',
        ],
        footer:
          '我们不会收集敏感个人信息，除非您自愿提供且必要（如健康相关信息用于特定职位匹配）。',
      },
    ],
  },
  {
    id: 'usage',
    title: '2. 我们如何使用您的信息',
    paragraphs: [
      '我们使用信息的主要目的是提供、维护和改进服务，包括：',
    ],
    items: [
      '创建和管理您的账户。',
      '匹配职位、推荐机会、模拟面试。',
      '处理支付和提供客户支持。',
      '发送通知、更新和营销信息（您可随时退订）。',
      '分析使用趋势、预防欺诈和改进服务。',
      '遵守法律义务。',
    ],
  },
  {
    id: 'sharing',
    title: '3. 我们如何分享您的信息',
    paragraphs: ['我们不会出售您的个人信息。我们可能在以下情况下分享信息：'],
    items: [
      '与服务提供商：如云存储、分析工具、支付处理器，这些第三方受保密协议约束。',
      '与合作伙伴：如雇主或招聘方，用于职位匹配（仅分享必要信息，且经您同意）。',
      '法律要求：如果法律要求、法院命令或保护权利，我们可能披露信息。',
      '业务转移：在合并、收购时，信息可能作为资产转移。',
      '您的同意：经您明确同意的其他分享。',
    ],
  },
  {
    id: 'storage',
    title: '4. 数据存储与国际传输',
    paragraphs: [
      '您的信息存储在安全的服务器上，可能位于中国或其他国家。我们采取措施确保跨境传输符合适用法律（如 GDPR 如果适用）。',
    ],
  },
  {
    id: 'security',
    title: '5. 数据安全',
    paragraphs: [
      '我们采用行业标准措施保护您的信息，包括加密、访问控制和定期审计。然而，没有系统是绝对安全的，我们无法保证绝对安全性。如果发生数据泄露，我们将及时通知您。',
    ],
  },
  {
    id: 'cookies',
    title: '6. Cookie 和跟踪技术',
    paragraphs: ['我们使用 Cookie 来提升用户体验：'],
    items: [
      '必要 Cookie：用于核心功能，如登录。',
      '性能 Cookie：分析网站性能。',
      '功能 Cookie：记住您的偏好。',
      '广告 Cookie：投放相关广告。',
    ],
    footer:
      '您可以通过浏览器设置管理 Cookie，但禁用可能影响服务功能。我们可能使用第三方服务如 Google Analytics。',
  },
  {
    id: 'rights',
    title: '7. 您的权利',
    paragraphs: ['根据适用法律，您有权：'],
    items: [
      '访问、更正或删除您的个人信息。',
      '反对或限制处理。',
      '撤回同意（不影响先前处理）。',
      '数据可移植性。',
    ],
    footer:
      '要行使权利，请联系我们（见第 9 节）。我们将在合理时间内响应。',
  },
  {
    id: 'links',
    title: '8. 第三方链接',
    paragraphs: [
      '服务可能包含第三方链接。我们不对其隐私实践负责。请查看他们的政策。',
    ],
  },
  {
    id: 'contact',
    title: '9. 联系我们',
    paragraphs: [
      '如果您对本政策有疑问，或需行使权利，请联系：',
    ],
  },
]
</script>

<template>
  <div class="page">
    <header class="header">
      <div class="header-inner">
        <div class="logo">
          <span class="logo-mark">P</span>
          <span class="logo-text">选我AI</span>
        </div>
        <div class="header-badge">隐私政策</div>
      </div>
    </header>

    <main class="main">
      <article class="policy">
        <header class="policy-header">
          <h1 class="policy-title">隐私政策</h1>
          <p class="policy-date">
            生效日期：<time :datetime="'2025-09-24'">{{ effectiveDate }}</time>
          </p>
        </header>

        <nav class="toc" aria-label="目录">
          <h2 class="toc-title">目录</h2>
          <ol class="toc-list">
            <li v-for="section in sections.filter((s) => s.title)" :key="section.id">
              <a :href="`#${section.id}`">{{ section.title }}</a>
            </li>
          </ol>
        </nav>

        <div class="policy-body">
          <section
            v-for="section in sections"
            :id="section.id"
            :key="section.id"
            class="section"
          >
            <h2 v-if="section.title" class="section-title">
              {{ section.title }}
            </h2>

            <p
              v-for="(para, i) in section.paragraphs"
              :key="`${section.id}-p-${i}`"
              class="paragraph"
            >
              {{ para }}
            </p>

            <template v-if="section.subsections">
              <div
                v-for="sub in section.subsections"
                :key="sub.title"
                class="subsection"
              >
                <h3 class="subsection-title">{{ sub.title }}</h3>
                <ul v-if="sub.items" class="list">
                  <li v-for="(item, i) in sub.items" :key="i">{{ item }}</li>
                </ul>
                <p v-if="sub.footer" class="paragraph footer-note">
                  {{ sub.footer }}
                </p>
              </div>
            </template>

            <ul v-else-if="section.items" class="list">
              <li v-for="(item, i) in section.items" :key="i">{{ item }}</li>
            </ul>

            <p v-if="section.footer" class="paragraph footer-note">
              {{ section.footer }}
            </p>

            <div
              v-if="section.id === 'contact'"
              class="contact-card"
            >
              <div class="contact-row">
                <span class="contact-label">电子邮件</span>
                <a :href="`mailto:${contactEmail}`" class="contact-link">
                  {{ contactEmail }}
                </a>
              </div>
              <div class="contact-row">
                <span class="contact-label">地址</span>
                <address class="contact-address">{{ contactAddress }}</address>
              </div>
              <p class="contact-note">
                我们将尽力解决您的关切。
              </p>
            </div>
          </section>

          <footer class="policy-footer">
            <p>感谢您信任 选我AI!</p>
          </footer>
        </div>
      </article>
    </main>
  </div>
</template>

<style scoped>
.page {
  min-height: 100vh;
  background: linear-gradient(160deg, #f0f4ff 0%, #f8f9fc 40%, #ffffff 100%);
  color: #1a1d26;
}

.header {
  position: sticky;
  top: 0;
  z-index: 10;
  background: rgba(255, 255, 255, 0.85);
  backdrop-filter: blur(12px);
  border-bottom: 1px solid rgba(0, 0, 0, 0.06);
}

.header-inner {
  max-width: 800px;
  margin: 0 auto;
  padding: 1rem 1.5rem;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.logo {
  display: flex;
  align-items: center;
  gap: 0.625rem;
}

.logo-mark {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 2rem;
  height: 2rem;
  border-radius: 0.5rem;
  background: linear-gradient(135deg, #4f6ef7 0%, #7c5cff 100%);
  color: #fff;
  font-weight: 700;
  font-size: 1rem;
}

.logo-text {
  font-weight: 600;
  font-size: 1.125rem;
  letter-spacing: -0.02em;
}

.header-badge {
  font-size: 0.8125rem;
  font-weight: 500;
  color: #4f6ef7;
  background: rgba(79, 110, 247, 0.1);
  padding: 0.375rem 0.75rem;
  border-radius: 999px;
}

.main {
  max-width: 800px;
  margin: 0 auto;
  padding: 2.5rem 1.5rem 4rem;
}

.policy {
  background: #fff;
  border-radius: 1rem;
  box-shadow:
    0 1px 3px rgba(0, 0, 0, 0.04),
    0 8px 24px rgba(79, 110, 247, 0.06);
  overflow: hidden;
}

.policy-header {
  padding: 2.5rem 2.5rem 1.5rem;
  border-bottom: 1px solid #eef0f5;
  background: linear-gradient(180deg, #fafbff 0%, #fff 100%);
}

.policy-title {
  font-size: 2rem;
  font-weight: 700;
  letter-spacing: -0.03em;
  line-height: 1.2;
  margin-bottom: 0.75rem;
}

.policy-date {
  font-size: 0.9375rem;
  color: #5c6370;
}

.policy-date time {
  font-weight: 500;
  color: #3d4450;
}

.toc {
  padding: 1.5rem 2.5rem;
  background: #f8f9fc;
  border-bottom: 1px solid #eef0f5;
}

.toc-title {
  font-size: 0.75rem;
  font-weight: 600;
  text-transform: uppercase;
  letter-spacing: 0.08em;
  color: #8b929e;
  margin-bottom: 0.75rem;
}

.toc-list {
  list-style: none;
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(220px, 1fr));
  gap: 0.375rem 1.5rem;
}

.toc-list a {
  display: block;
  padding: 0.25rem 0;
  font-size: 0.875rem;
  color: #4f6ef7;
  text-decoration: none;
  transition: color 0.15s;
}

.toc-list a:hover {
  color: #3a56d4;
  text-decoration: underline;
}

.policy-body {
  padding: 2rem 2.5rem 2.5rem;
}

.section {
  margin-bottom: 2.25rem;
  scroll-margin-top: 5rem;
}

.section:last-of-type {
  margin-bottom: 0;
}

.section-title {
  font-size: 1.25rem;
  font-weight: 600;
  color: #1a1d26;
  margin-bottom: 1rem;
  padding-bottom: 0.5rem;
  border-bottom: 2px solid #eef0f5;
}

.subsection {
  margin: 1.25rem 0 1.5rem;
}

.subsection-title {
  font-size: 1rem;
  font-weight: 600;
  color: #3d4450;
  margin-bottom: 0.625rem;
}

.paragraph {
  font-size: 0.9375rem;
  line-height: 1.75;
  color: #3d4450;
  margin-bottom: 0.875rem;
}

.paragraph:last-child {
  margin-bottom: 0;
}

.footer-note {
  margin-top: 0.75rem;
  padding-left: 0.875rem;
  border-left: 3px solid #e0e6ff;
}

.list {
  margin: 0.5rem 0 0.875rem;
  padding-left: 1.25rem;
}

.list li {
  font-size: 0.9375rem;
  line-height: 1.75;
  color: #3d4450;
  margin-bottom: 0.375rem;
}

.list li::marker {
  color: #4f6ef7;
}

.contact-card {
  margin-top: 1rem;
  padding: 1.25rem 1.5rem;
  background: #f8f9fc;
  border-radius: 0.75rem;
  border: 1px solid #eef0f5;
}

.contact-row {
  display: flex;
  flex-wrap: wrap;
  gap: 0.5rem 1rem;
  margin-bottom: 0.875rem;
}

.contact-row:last-of-type {
  margin-bottom: 0;
}

.contact-label {
  flex: 0 0 4.5rem;
  font-size: 0.8125rem;
  font-weight: 600;
  color: #8b929e;
  text-transform: uppercase;
  letter-spacing: 0.04em;
}

.contact-link {
  font-size: 0.9375rem;
  color: #4f6ef7;
  text-decoration: none;
  font-weight: 500;
}

.contact-link:hover {
  text-decoration: underline;
}

.contact-address {
  font-size: 0.9375rem;
  line-height: 1.6;
  color: #3d4450;
  font-style: normal;
  flex: 1;
  min-width: 200px;
}

.contact-note {
  margin-top: 1rem;
  padding-top: 1rem;
  border-top: 1px solid #eef0f5;
  font-size: 0.9375rem;
  color: #5c6370;
}

.policy-footer {
  margin-top: 2.5rem;
  padding-top: 1.5rem;
  border-top: 1px solid #eef0f5;
  text-align: center;
}

.policy-footer p {
  font-size: 1rem;
  font-weight: 500;
  color: #4f6ef7;
}

@media (max-width: 640px) {
  .main {
    padding: 1rem 1rem 2.5rem;
  }

  .policy-header,
  .toc,
  .policy-body {
    padding-left: 1.25rem;
    padding-right: 1.25rem;
  }

  .policy-title {
    font-size: 1.625rem;
  }

  .toc-list {
    grid-template-columns: 1fr;
  }
}
</style>
