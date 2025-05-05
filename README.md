# MENA 地区风险采集与分析工具

## 📘 项目简介

本项目为一个基于 Python 编写的新闻网页数据抓取与风险分析工具，目标是自动采集中东与北非（MENA）国家的新闻数据，匹配关键词并分类为三大类风险：
- **政治（社会）风险**
- **经济风险**
- **自然风险**

数据来源包括：
- [TAP - 突尼斯通讯社](https://www.tap.info.tn/)
- [MENA - 埃及中东通讯社](https://www.mena.org.eg/)
- [阿尔及利亚通讯社](https://www.aps.dz/)
- [摩洛哥通讯社](https://www.mapnews.ma/)

主要功能：
1. 自动抓取新闻网页；
2. 使用 BeautifulSoup 解析页面内容；
3. 匹配关键词并进行风险分类；
4. 使用 pandas 生成结构化表格；
5. 绘制风险指数柱状图；
6. 导出分析结果为 Excel。

---

## 📦 安装依赖

将下列内容保存为 `requirements.txt` 文件：

```txt
beautifulsoup4
cmasher
matplotlib
pandas
requests
scienceplots
selenium
scikit-learn
urllib3
webdriver-manager
```

然后运行以下命令安装依赖：

```bash
pip install -r requirements.txt
```

建议使用虚拟环境运行项目：

```bash
conda create -n zdtxs python=3.10
conda activate zdtxs
pip install -r requirements.txt
```

---

## 📊 输出示例

程序将输出：
- 一个 Excel 文件（如 `Tunisia_Risks.xlsx`）；
- 若干图表（如 `Risk_Index_Plot.png`）展示各类风险指数；
- 可选的雷达图进行国家对比分析。

---

## 📁 文件说明

| 文件名 | 描述 |
|--------|------|
| `zdtxs.ipynb` | 主程序 Notebook，包含数据采集、分析与可视化 |
| `requirements.txt` | 所需库依赖文件 |
| `output/` | 结果文件（Excel、图表）输出目录 |

---

## 📮 联系方式

如有问题，欢迎反馈或提交 issue。
