# Awesome-Exposure-Management-Platform

# 顶级暴露管理平台生态系统



**精选 SaaS 产品与开源 GitHub 项目列表**

*聚焦攻击面管理、漏洞优先级排序、CAASM 与风险修复*

**最后更新：2026 年 9 月**



本仓库追踪**暴露管理**领域的知名 **SaaS 平台**与**开源项目**。这些工具帮助安全团队统一云、本地和代码环境中的风险数据，基于真实攻击上下文验证和优先级排序暴露面，并加速修复工作流。



**示例**包括 Tenable One、Qualys TotalCloud、Rapid7 Exposure Command、Wiz、Palo Alto Cortex Exposure Management、Microsoft Security Exposure Management、Armis、Axonius、runZero 和 Noetic Cyber（该领域的领先者）。



**开源重点**：暴露管理领域的开源生态**尚处于早期阶段**。商业平台（Wiz、Tenable、Qualys）主导市场，开源替代方案主要集中在**攻击面发现**（runZero 的部分功能、Nmap 生态）、**漏洞扫描**（OpenVAS、Nuclei）和**资产数据整合**层面。**XORCISM** 是搜索结果中唯一明确以“开源统一暴露管理平台”定位的项目，但处于早期阶段。本列表诚实地记录了这一现状。



欢迎贡献！提交 PR 以添加/更新条目。保持描述事实性，并链接到官方网站。



## 目录



- [SaaS/托管平台](#saas托管平台)

- [开源 GitHub 项目](#开源github项目)

- [如何贡献](#如何贡献)

- [免责声明](#免责声明)



## SaaS/托管平台



- **[Tenable One](https://www.tenable.com/)**

  AI 驱动的暴露管理平台，统一资产、漏洞和攻击面数据。支持第三方数据连接器，将非 Tenable 工具数据汇入统一视图，提供自定义风险仪表板以识别有毒风险组合（未修补漏洞 + 错误配置 + 过度权限）。



- **[Qualys TotalCloud](https://www.qualys.com/)**

  CNAPP 平台，提供 TruRisk Insights 统一风险视图。功能包括 **Attack Path 分析**（映射攻击路径和爆炸半径）、**Cloud Workflow Automation**（无代码 QFlow Playbook 自动化修复流程）、3 步多租户引导 。



- **[Rapid7 Exposure Command](https://www.rapid7.com/)**

  端到端漏洞与暴露管理平台。**Remediation Hub** 支持自动化修复工作流、补偿控制评估、第三方漏洞集成（Tenable、Qualys、Wiz）。超过 275 个开箱即用集成，500+ 预建自动化工作流。IDC MarketScape 2025 暴露管理领导者 。



- **[Wiz](https://www.wiz.io/)**

  云安全平台，2025 年 GA 的 **Exposure Management** 功能统一了 **UVM**（统一漏洞管理）和 **ASM**（攻击面管理）。基于 Wiz Security Graph 关联代码到云上下文，支持外部暴露验证和真实可利用性验证（模拟攻击）。



- **[Palo Alto Cortex Exposure Management](https://www.paloaltonetworks.com/)**

  Cortex XDR 中的暴露管理模块。整合 Palo Alto 传感器（Cortex Agent、ASM、Attack Surface Testing、Network Scanner）与第三方扫描器（Qualys、Rapid7、Tenable、CrowdStrike）。提供精度过滤、补偿控制识别、自动化修复内容包 。



- **[Microsoft Security Exposure Management](https://www.microsoft.com/)**

  集成于 Microsoft Defender XDR 门户。基于**企业暴露图**（Enterprise Exposure Graph）构建，自动生成**攻击路径**，识别关键资产（域控制器、敏感数据库、特权角色）。支持外部数据连接器（预览版）。



- **[Armis](https://www.armis.com/)**

  Armis Centrix 平台，基于 AI 驱动的资产智能引擎。覆盖 IT、IoT、IoMT、OT、云和移动资产。提供**Cyber Exposure Management**，AI 驱动的风险评分和去重，实时检测异常行为和活跃利用模式 。



- **[Axonius](https://www.axonius.com/)**

  资产云平台，整合 1000+ 数据源提供统一资产数据模型。模块包括 Cyber Assets、SaaS Applications、Identities、**Exposures**（漏洞聚合与优先级）、Software Assets。**Workflows** 自动化补丁编排、告警富化、身份生命周期管理 。



- **[runZero](https://www.runzero.com/)**

  攻击面管理平台，无凭据网络扫描。提供完整资产可见性（含非托管和 rogue 设备），**异常值评分**（outlier score 0-5）识别不寻常资产，Findings 聚合漏洞、错误配置和最佳实践为优先级列表 。



- **[Noetic Cyber](https://www.noeticcyber.com/)**

  CAASM 平台，整合多源数据提供资产暴露和网络风险的全面视图。与 Lansweeper 集成增强资产可见性，自动化优先级排序修复工作流 。



## 开源 GitHub 项目



- **[XORCISM](https://github.com/XORCISM-AI/XORCISM)**

  搜索结果中唯一明确以**开源统一暴露管理平台**定位的项目。覆盖 NIST CSF 2.0 治理、辅助渗透测试（AI 驱动）、暴露融合评分。提供只读 REST API（`/api/v1/exposures`）用于 SIEM 和自动化。**早期项目**，需添加 LICENSE 文件明确条款 。



- **[OpenVAS](https://github.com/greenbone/openvas-scanner)**

  开源漏洞扫描器（Greenbone 社区版）。提供超过 50,000 个网络漏洞测试，支持认证和无认证扫描。可作为暴露管理计划中**漏洞发现层**的开源基础。



- **[Nuclei](https://github.com/projectdiscovery/nuclei)**

  基于模板的快速漏洞扫描器，由 ProjectDiscovery 开发。拥有社区驱动的模板库，覆盖 CVE、错误配置、暴露面板等。适合作为**持续攻击面发现**的开源工具。



- **[Nmap](https://github.com/nmap/nmap)**

  网络发现和端口扫描的事实标准。提供主机发现、端口扫描、服务/版本检测、OS 指纹识别。是多数商业 ASM 平台底层的发现引擎。



- **[OWASP Amass](https://github.com/owasp-amass/amass)**

  开源攻击面映射工具。通过主动和被动侦察绘制组织的外部网络资产和 DNS 基础设施。



- **[Katana](https://github.com/projectdiscovery/katana)**

  下一代爬虫和蜘蛛框架，用于发现 Web 应用端点。适合作为暴露管理中**Web 资产发现**的组件。



- **[OWASP Dependency-Track](https://github.com/DependencyTrack/dependency-track)**

  软件成分分析平台，持续监控 SBOM 中的漏洞。适合作为**代码/依赖暴露**的发现层。



### 其他强开源选项



- **漏洞扫描**：**OpenVAS**、**Nuclei**、**Trivy**（容器和文件系统漏洞扫描）。

- **资产发现**：**Nmap**、**OWASP Amass**、**Masscan**（高速端口扫描）。

- **暴露面映射**：**Katana**（Web 爬虫）、**OWASP ZAP**（动态应用安全测试）。

- **SBOM 与依赖**：**Dependency-Track**、**Syft**（SBOM 生成）、**Grype**（漏洞扫描）。



**构建自定义系统的框架**：使用 **Nmap** + **OWASP Amass** 进行资产发现，**OpenVAS** + **Nuclei** 进行漏洞扫描，**Dependency-Track** + **Trivy** 进行代码/容器暴露分析，**Katana** 进行 Web 攻击面映射。数据层可结合 **PostgreSQL** 存储资产和发现，**Elasticsearch** 支持搜索。**注意**：完整暴露管理需要的**攻击路径关联、优先级排序算法、修复工作流编排**在开源生态中尚无成熟实现，需大量自定义开发。



## 如何贡献



1. Fork 仓库。

2. 在 `README.md` 中添加/编辑条目（遵循现有格式）。

3. 包含：名称、链接、1-2 句描述，以及是 SaaS 还是开源。

4. 提交 PR 并附简短说明。



如果你觉得这个仓库有用，请点星！



## 免责声明



- 这是一个**社区精选**列表——并非详尽无遗，也不构成认可。

- 暴露管理平台处理敏感的资产和漏洞数据；确保适当的访问控制和数据保护。

- **开源现实**：暴露管理是安全领域**开源生态最薄弱的环节之一**。商业平台（Wiz、Tenable、Qualys、Rapid7）在攻击路径分析、风险上下文关联和自动化修复方面有多年积累。开源工具在**发现层**（Nmap、OpenVAS、Nuclei）成熟可用，但**统一暴露管理平台**的开源替代方案几乎不存在。**XORCISM** 是最接近的开源尝试，但处于早期阶段，生产就绪度未知 。



---



**为安全工程师、漏洞管理团队、SOC 分析师和安全架构师打造。**

让暴露管理更开放、透明、可操作。
