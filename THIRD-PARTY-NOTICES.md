# 第三方组件与数据来源许可清单

本文件的 HTML 内嵌了第三方代码与数据。**完整的许可全文（MIT、BSD-3-Clause、Apache-2.0）也已写入 HTML 页面页脚的「许可与数据来源」折叠项**——也就是说，即使只分发那一个 HTML 文件，许可与署名信息同样随文件一起分发，不会遗漏。

---

## 一、内嵌代码库

| 组件 | 版本 | 许可 | 用途 |
|---|---|---|---|
| [KaTeX](https://katex.org) | 0.16.22 | MIT | 化学方程式与公式排版 |
| [smiles-drawer](https://github.com/reymond-group/smilesDrawer) | 2.1.7 | MIT | 有机分子二维结构式 |
| [ts-fsrs](https://github.com/open-spaced-repetition/ts-fsrs) | 5.2.1 | MIT | 生词本的间隔重复调度 |
| [3Dmol.js](https://3dmol.org) | 2.4.2 | BSD-3-Clause | 三维分子结构显示 |
| [uPlot](https://github.com/leeoniya/uPlot) | 1.6.32 | MIT | 周期性趋势交互图表 |
| CMU Pronouncing Dictionary | — | BSD 风格 | 英文名称发音数据 |

### 各自的版权行

- **KaTeX**：Copyright (c) 2013-2020 Khan Academy and other contributors。随包分发的字体同样以 MIT 分发；`contrib/mhchem` 扩展随 KaTeX 包分发，`\ce{}` 化学式语法源自 Martin Hensel 的 mhchem。
- **smiles-drawer**：Copyright (c) 2017 GDB / Reymond Research Group。其打包文件内含 **chroma.js**（Apache-2.0，含 colorbrewer2.org 配色，Copyright (c) 2002 Cynthia Brewer, Mark Harrower, and The Pennsylvania State University）。
- **ts-fsrs**：Copyright (c) 2026 Open Spaced Repetition
- **3Dmol.js**：Copyright (c) 2014, University of Pittsburgh and contributors, All rights reserved.
- **uPlot**：Copyright (c) 2022 Leon Sorokin
- **CMU Pronouncing Dictionary**：Copyright (C) 1993-2015 Carnegie Mellon University. All rights reserved.
- **中文字形**：不内嵌任何字体，中文使用系统字体栈。

---

## 二、内嵌数据

### 2.1 元素与化学数据

| 内容 | 来源 | 许可 |
|---|---|---|
| 元素基础性质 | 原页面数据 + [PubChem](https://pubchem.ncbi.nlm.nih.gov) | 美国政府作品 |
| 原子半径、离子半径、天然同位素丰度 | [mendeleev](https://github.com/lmmentel/mendeleev) 1.3.0 | MIT，Copyright (c) 2015 Lukasz Mentel |
| 标准生成焓 | [chemicals](https://github.com/CalebBell/chemicals)（原始数据来自 CRC Handbook 与 JANAF） | MIT，Copyright (C) 2016-2021 Caleb Bell |
| GHS 危险分类 | PubChem GHS Classification | 美国政府作品 |
| GHS 象形图 | Wikimedia Commons | 公有领域 |
| 红外吸收峰位（10 个化合物） | NIST Chemistry WebBook 的 MSDC-IR 数据集 | 美国政府作品 |
| 三维分子结构（21 个） | PubChem 3D SDF | 美国政府作品 |

### 2.2 化合物物理性质字段（共 1177 个字段）

| 来源数据库 | 字段数 | 许可依据 |
|---|---|---|
| Hazardous Substances Data Bank (HSDB) | 393 | 美国国家医学图书馆（NLM）作品，需按 NLM 条款致谢 |
| PAC Chemical Database, U.S. Department of Energy | 150 | 美国联邦机构作品，不受美国版权保护 |
| EPA Chemical Data Reporting (CDR) | 97 | 美国联邦机构作品，不受美国版权保护 |
| The National Institute for Occupational Safety and Health (NIOSH) | 46 | 美国联邦机构作品，不受美国版权保护 |
| Occupational Safety and Health Administration (OSHA) | 36 | 美国联邦机构作品，不受美国版权保护 |
| CAMEO Chemicals | 33 | 美国联邦机构作品，不受美国版权保护 |
| EU Food Improvement Agents | 11 | 【欧盟】**CC BY 4.0**（Committee Decision 2011/833/EU，已核实） |
| Agency for Toxic Substances and Disease Registry (ATSDR) | 1 | 美国联邦机构作品，不受美国版权保护 |
| PubChem 直接查询（`rest/pug/compound/name/.../JSON`） | 410 | 美国政府作品 |

### 2.3 NLM 数据的使用要求（重要）

Hazardous Substances Data Bank（HSDB）由美国国家医学图书馆（NLM）编制。NLM 的[数据下载条款](https://www.nlm.nih.gov/databases/download/terms_and_conditions.html)原文要求使用方：

1. **致谢**：以清晰显著的方式注明 "Courtesy of the U.S. National Library of Medicine"；
2. **不得暗示背书**：不得表明或暗示 NLM 认可其产品或服务；
3. **时效说明**：再分发者须保留最新版本，或清晰说明所分发内容**可能不是 NLM 当前的最新版本**。

本文件已在页脚的许可区块中一并写明这三条。原文摘录：

> Users of the data agree to: acknowledge NLM as the source of the data by including the phrase "Courtesy of the U.S. National Library of Medicine" in a clear and conspicuous manner, not indicate or imply that NLM has endorsed its products/services/applications. Users who republish or redistribute the data (services, products or raw data) agree to: maintain the most current version of all distributed data, or make known in a clear and conspicuous manner that the products/services/applications do not reflect the most current/accurate data available from NLM.

### 2.4 EU 数据的依据

欧盟委员会法律声明原文（[来源](https://commission.europa.eu/legal-notice_en)）：

> © European Union, 1995-2026 … Unless otherwise indicated, content owned by the EU on this website is licensed under the Creative Commons Attribution 4.0 International (CC BY 4.0) licence. This means that reuse is allowed, provided appropriate credit is given and changes are indicated.

### 2.5 已移除的第三方数据

以下来源曾出现在早期版本中，**均已在发布前移除**（合计 524 个字段）：

| 来源 | 字段数 | 移除原因 |
|---|---|---|
| Haz-Map | 285 | **第三方所有**（作者 Jay A. Brown），并非美国政府作品；由 NLM 托管只是基于授权协议，而该协议已于 2019 年前后终止（[依据](https://m.wikidata.org/wiki/Wikidata:Property_proposal/Haz-Map_ID)），且未找到允许再分发的明确声明 |
| ILO-WHO International Chemical Safety Cards (ICSCs) | 172 | ILO 的开放获取政策只覆盖 2023-05-03 之后发布的出版物；ICSC 属此前出版物，且卡片与相关页面均无授权声明 |
| DrugBank | 21 | CC BY-NC 4.0，含非商业限制 |
| Human Metabolome Database (HMDB) | 20 | 同上 |
| Cosmetic Ingredient Review (CIR) | 18 | 报告受版权保护 |
| Toxin and Toxin Target Database (T3DB) | 7 | 非商业限制 |
| NORMAN Suspect List Exchange | 1 | 条款未明确 |

### 2.6 关于 PubChem 的提醒

PubChem 由 NCBI/NLM 维护，[政策](https://www.ncbi.nlm.nih.gov/home/about/policies/)声明美国政府创建的信息属公有领域，可自由分发与复制，建议致谢 NLM。但 PubChem 同时收录大量第三方贡献的数据（上表中的 Haz-Map、ICSC、DrugBank、HMDB 都是经 PubChem 收录而非免费数据）。**"能从 PubChem 取到"不等于"可以自由再分发"**——本文件只保留能确认是政府作品或经核实许可的部分。

---

## 三、许可全文

以下全文**同时内嵌在 HTML 页脚的「许可与数据来源」折叠项中**，此处再列一遍便于单独查阅。

### MIT License（KaTeX、smiles-drawer、ts-fsrs、uPlot、mendeleev、chemicals）

```
MIT License

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

### BSD 3-Clause License（3Dmol.js）

```
3Dmol.js incorporates code from GLmol, Three.js, and jQuery and
is licensed under a BSD-3-Clause license.

* 3Dmol.js
	Copyright (c) 2014, University of Pittsburgh and contributors
	All rights reserved.

	Redistribution and use in source and binary forms, with or without 
	modification, are permitted provided that the following conditions are met:

	1. Redistributions of source code must retain the above copyright 
	notice, this list of conditions and the following disclaimer.

	2. Redistributions in binary form must reproduce the above copyright 
	notice, this list of conditions and the following disclaimer in the 
	documentation and/or other materials provided with the distribution.

	3. Neither the name of the copyright holder nor the names of its 
	contributors may be used to endorse or promote products derived from 
	this software without specific prior written permission.

	THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS 
	"AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT 
	LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A 
	PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
	HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, 
	SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED 
	TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR 
	PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF 
	LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING 
	NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS 
	SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.

* GLmol
 GLmol - Molecular Viewer on WebGL/Javascript (0.47)
  (C) Copyright 2011-2012, biochem_fan
      License: dual license of MIT or LGPL3

  Contributors:
    Robert Hanson for parseXYZ, deferred instantiation



* Three.js 
     https://github.com/mrdoob/three.js

     Copyright (c) 2010-2012 three.js Authors. All rights reserved.

     Permission is hereby granted, free of charge, to any person obtaining a copy
     of this software and associated documentation files (the "Software"), to deal
     in the Software without restriction, including without limitation the rights
     to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
     copies of the Software, and to permit persons to whom the Software is
     furnished to do so, subject to the following conditions:

     The above copyright notice and this permission notice shall be included in
     all copies or substantial portions of the Software.

     THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
     IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
     FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
     AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
     LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
     OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
     THE SOFTWARE.

* jQuery
     http://jquery.org/

     Copyright (c) 2011 John Resig

     Permission is hereby granted, free of charge, to any person obtaining
     a copy of this software and associated documentation files (the
     "Software"), to deal in the Software without restriction, including
     without limitation the rights to use, copy, modify, merge, publish,
     distribute, sublicense, and/or sell copies of the Software, and to
     permit persons to whom the Software is furnished to do so, subject to
     the following conditions:

     The above copyright notice and this permission notice shall be
     included in all copies or substantial portions of the Software.

     THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
     EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
     MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
     NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
     LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
     OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
     WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Apache License 2.0（smiles-drawer 内含的 chroma.js）

```
Apache License
                           Version 2.0, January 2004
                        http://www.apache.org/licenses/

   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION

   1. Definitions.

      "License" shall mean the terms and conditions for use, reproduction,
      and distribution as defined by Sections 1 through 9 of this document.

      "Licensor" shall mean the copyright owner or entity authorized by
      the copyright owner that is granting the License.

      "Legal Entity" shall mean the union of the acting entity and all
      other entities that control, are controlled by, or are under common
      control with that entity. For the purposes of this definition,
      "control" means (i) the power, direct or indirect, to cause the
      direction or management of such entity, whether by contract or
      otherwise, or (ii) ownership of fifty percent (50%) or more of the
      outstanding shares, or (iii) beneficial ownership of such entity.

      "You" (or "Your") shall mean an individual or Legal Entity
      exercising permissions granted by this License.

      "Source" form shall mean the preferred form for making modifications,
      including but not limited to software source code, documentation
      source, and configuration files.

      "Object" form shall mean any form resulting from mechanical
      transformation or translation of a Source form, including but
      not limited to compiled object code, generated documentation,
      and conversions to other media types.

      "Work" shall mean the work of authorship, whether in Source or
      Object form, made available under the License, as indicated by a
      copyright notice that is included in or attached to the work
      (an example is provided in the Appendix below).

      "Derivative Works" shall mean any work, whether in Source or Object
      form, that is based on (or derived from) the Work and for which the
      editorial revisions, annotations, elaborations, or other modifications
      represent, as a whole, an original work of authorship. For the purposes
      of this License, Derivative Works shall not include works that remain
      separable from, or merely link (or bind by name) to the interfaces of,
      the Work and Derivative Works thereof.

      "Contribution" shall mean any work of authorship, including
      the original version of the Work and any modifications or additions
      to that Work or Derivative Works thereof, that is intentionally
      submitted to Licensor for inclusion in the Work by the copyright owner
      or by an individual or Legal Entity authorized to submit on behalf of
      the copyright owner. For the purposes of this definition, "submitted"
      means any form of electronic, verbal, or written communication sent
      to the Licensor or its representatives, including but not limited to
      communication on electronic mailing lists, source code control systems,
      and issue tracking systems that are managed by, or on behalf of, the
      Licensor for the purpose of discussing and improving the Work, but
      excluding communication that is conspicuously marked or otherwise
      designated in writing by the copyright owner as "Not a Contribution."

      "Contributor" shall mean Licensor and any individual or Legal Entity
      on behalf of whom a Contribution has been received by Licensor and
      subsequently incorporated within the Work.

   2. Grant of Copyright License. Subject to the terms and conditions of
      this License, each Contributor hereby grants to You a perpetual,
      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
      copyright license to reproduce, prepare Derivative Works of,
      publicly display, publicly perform, sublicense, and distribute the
      Work and such Derivative Works in Source or Object form.

   3. Grant of Patent License. Subject to the terms and conditions of
      this License, each Contributor hereby grants to You a perpetual,
      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
      (except as stated in this section) patent license to make, have made,
      use, offer to sell, sell, import, and otherwise transfer the Work,
      where such license applies only to those patent claims licensable
      by such Contributor that are necessarily infringed by their
      Contribution(s) alone or by combination of their Contribution(s)
      with the Work to which such Contribution(s) was submitted. If You
      institute patent litigation against any entity (including a
      cross-claim or counterclaim in a lawsuit) alleging that the Work
      or a Contribution incorporated within the Work constitutes direct
      or contributory patent infringement, then any patent licenses
      granted to You under this License for that Work shall terminate
      as of the date such litigation is filed.

   4. Redistribution. You may reproduce and distribute copies of the
      Work or Derivative Works thereof in any medium, with or without
      modifications, and in Source or Object form, provided that You
      meet the following conditions:

      (a) You must give any other recipients of the Work or
          Derivative Works a copy of this License; and

      (b) You must cause any modified files to carry prominent notices
          stating that You changed the files; and

      (c) You must retain, in the Source form of any Derivative Works
          that You distribute, all copyright, patent, trademark, and
          attribution notices from the Source form of the Work,
          excluding those notices that do not pertain to any part of
          the Derivative Works; and

      (d) If the Work includes a "NOTICE" text file as part of its
          distribution, then any Derivative Works that You distribute must
          include a readable copy of the attribution notices contained
          within such NOTICE file, excluding those notices that do not
          pertain to any part of the Derivative Works, in at least one
          of the following places: within a NOTICE text file distributed
          as part of the Derivative Works; within the Source form or
          documentation, if provided along with the Derivative Works; or,
          within a display generated by the Derivative Works, if and
          wherever such third-party notices normally appear. The contents
          of the NOTICE file are for informational purposes only and
          do not modify the License. You may add Your own attribution
          notices within Derivative Works that You distribute, alongside
          or as an addendum to the NOTICE text from the Work, provided
          that such additional attribution notices cannot be construed
          as modifying the License.

      You may add Your own copyright statement to Your modifications and
      may provide additional or different license terms and conditions
      for use, reproduction, or distribution of Your modifications, or
      for any such Derivative Works as a whole, provided Your use,
      reproduction, and distribution of the Work otherwise complies with
      the conditions stated in this License.

   5. Submission of Contributions. Unless You explicitly state otherwise,
      any Contribution intentionally submitted for inclusion in the Work
      by You to the Licensor shall be under the terms and conditions of
      this License, without any additional terms or conditions.
      Notwithstanding the above, nothing herein shall supersede or modify
      the terms of any separate license agreement you may have executed
      with Licensor regarding such Contributions.

   6. Trademarks. This License does not grant permission to use the trade
      names, trademarks, service marks, or product names of the Licensor,
      except as required for reasonable and customary use in describing the
      origin of the Work and reproducing the content of the NOTICE file.

   7. Disclaimer of Warranty. Unless required by applicable law or
      agreed to in writing, Licensor provides the Work (and each
      Contributor provides its Contributions) on an "AS IS" BASIS,
      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
      implied, including, without limitation, any warranties or conditions
      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
      PARTICULAR PURPOSE. You are solely responsible for determining the
      appropriateness of using or redistributing the Work and assume any
      risks associated with Your exercise of permissions under this License.

   8. Limitation of Liability. In no event and under no legal theory,
      whether in tort (including negligence), contract, or otherwise,
      unless required by applicable law (such as deliberate and grossly
      negligent acts) or agreed to in writing, shall any Contributor be
      liable to You for damages, including any direct, indirect, special,
      incidental, or consequential damages of any character arising as a
      result of this License or out of the use or inability to use the
      Work (including but not limited to damages for loss of goodwill,
      work stoppage, computer failure or malfunction, or any and all
      other commercial damages or losses), even if such Contributor
      has been advised of the possibility of such damages.

   9. Accepting Warranty or Additional Liability. While redistributing
      the Work or Derivative Works thereof, You may choose to offer,
      and charge a fee for, acceptance of support, warranty, indemnity,
      or other liability obligations and/or rights consistent with this
      License. However, in accepting such obligations, You may act only
      on Your own behalf and on Your sole responsibility, not on behalf
      of any other Contributor, and only if You agree to indemnify,
      defend, and hold each Contributor harmless for any liability
      incurred by, or claims asserted against, such Contributor by reason
      of your accepting any such warranty or additional liability.

   END OF TERMS AND CONDITIONS

   APPENDIX: How to apply the Apache License to your work.

      To apply the Apache License to your work, attach the following
      boilerplate notice, with the fields enclosed by brackets "[]"
      replaced with your own identifying information. (Don't include
      the brackets!)  The text should be enclosed in the appropriate
      comment syntax for the file format. We also recommend that a
      file or class name and description of purpose be included on the
      same "printed page" as the copyright notice for easier
      identification within third-party archives.

   Copyright [yyyy] [name of copyright owner]

   Licensed under the Apache License, Version 2.0 (the "License");
   you may not use this file except in compliance with the License.
   You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.
```

---

## 四、核对时查阅的官方页面

| 页面 | 用途 |
|---|---|
| [NLM 数据下载条款](https://www.nlm.nih.gov/databases/download/terms_and_conditions.html) | 确认 HSDB 可再分发及致谢要求 |
| [欧盟委员会法律声明](https://commission.europa.eu/legal-notice_en) | 确认 EU 数据为 CC BY 4.0 |
| [ILO 权利与许可](https://www.ilo.org/rights-and-permissions) | 确认 ICSC 授权状态（据此移除） |
| [NCBI/NLM 政策](https://www.ncbi.nlm.nih.gov/home/about/policies/) | 确认 PubChem 数据的地位 |
| [Wikidata Haz-Map 属性提案](https://m.wikidata.org/wiki/Wikidata:Property_proposal/Haz-Map_ID) | 确认 Haz-Map 为第三方所有、NLM 授权已终止（据此移除） |
