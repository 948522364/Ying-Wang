
![工资及相关因素](Personal%20salary%20and%20other%20factors.png)

## 项目背景
该数据集包含了个人的工资及其相关的社会、经济因素，如年龄、婚姻状态、种族、教育程度、健康状况等。
在学习分析的角度下，数据可以用于探索不同学习、教育背景的人群对其工资带来的影响，并判断是否符合我们普遍认为的学习越高，工资越高的说法。

该数据集也可以用于研究其他的方向,例如：

- **地区与种族的薪资差异分析**：不同地区、种族的工资水平差异及其背后的原因。
- **健康状况与职业发展的关系**：健康状况是否对工资有显著影响。

---

## 徽章 (Badges)
![GitHub last commit](https://img.shields.io/github/last-commit/948522364/Ying-Wang)
![License](https://img.shields.io/github/license/948522364/Ying-Wang)
![GitHub contributors](https://img.shields.io/github/contributors/948522364/Ying-Wang)

---

## 数据集概述
- **数据集名称**: 个人工资及相关因素数据集
- **记录数量**: 3000 条记录
- **变量数量**: 11 个变量
- **文件格式**: CSV

---

## DDI 标准应用

### 1. 概述
该数据集包含了有关个人工资及其相关因素的信息，数据结构化且表格化，因此使用了 **Data Documentation Initiative (DDI)** 标准来描述和记录该数据集，确保其符合社会、行为和经济科学数据的要求。

### 2. DDI 标准的使用
DDI 标准帮助我们提供详细的元数据，涵盖了：
- **数据生命周期管理**：从数据创建到存档和重用的全过程管理。
- **变量级元数据**：为每个变量提供详细的描述，包括数据类型、测量单位和允许的取值。
- **文档化**：为用户和研究人员提供清晰的文档，以便他们理解数据集的结构和内容。


---

### 3. 数据字典
以下是数据集中的每个变量及其定义，遵循 DDI 标准：

| Variable Name | Readable Variable Name | Measurement Units | Allowed Values | Definition of the Variable | Synonyms for the Variable Name | Description of the Variable | Other Resources |
| ------------- | ---------------------- | ----------------- | -------------- | -------------------------- | ----------------------------- | --------------------------- | --------------- |
| year          | Year                   | Year              | 2003-2006      | Year of data collection     | Collection Year               | Year the data was recorded, ranging from 2003 to 2006. | N/A |
| age           | Age                    | Years             | 18-80          | Age of the individual at the time of data collection | Individual Age | Age of the individuals in the dataset, representing a wide age range. | N/A |
| maritl        | Marital Status          | N/A               | 1-5            | Marital status of the individual (1: Never Married, 2: Married, 3: Widowed, 4: Divorced, 5: Separated) | Marital Condition | Represents the marital status with different categories. | N/A |
| race          | Race                   | N/A               | 1-3            | Race of the individual (1: White, 2: Black, 3: Asian) | Ethnicity | Shows the race of the individual from the given categories. | N/A |
| education     | Education Level         | N/A               | 1-5            | Highest educational attainment of the individual (1: < HS Grad, 2: HS Grad, 3: Some College, 4: College Grad, 5: Advanced Degree) | Schooling Level | Education level achieved by the individual, classified into 5 categories. | N/A |
| region        | Region                 | N/A               | 1-4            | Region where the individual resides (1: Northeast, 2: Middle Atlantic, 3: South, 4: West) | Geographical Area | Region of residence, representing different geographical divisions. | N/A |
| jobclass      | Job Class              | N/A               | 1-2            | Type of job class (1: Industrial, 2: Information) | Job Type | The industry type or sector in which the individual works. | N/A |
| health        | Health Status          | N/A               | 1-2            | Health status of the individual (1: <=Good, 2: >=Very Good) | Physical Health | The health status is reported as either good or very good. | N/A |
| health_ins    | Health Insurance       | N/A               | 1-2            | Whether the individual has health insurance (1: Yes, 2: No) | Health Coverage | Shows if the individual has health insurance coverage. | N/A |
| logwage       | Log of Wage            | Log (base 10)     | -∞ to ∞        | Logarithm of the wage (log base 10 of actual wage) | Wage Logarithm | Logarithmic transformation of the wage for better data distribution. | N/A |
| wage          | Wage                   | USD               | 0 to ∞         | Actual wage earned by the individual | Salary | The actual wage in US dollars earned by the individual. | N/A |

---

### 4. 数据收集方法
- **数据来源**: 数据集来源于公开的个人薪资调查。
- **数据收集时间**: 数据反映了 2003 年至 2006 年的个人工资情况。
- **数据处理**: 我们进行了基本的数据清理，处理了缺失值，并确保各列的一致性。没有发现明显的异常值。

---

### 5. 引用和使用
- **DDI 标准**: 该数据集使用 DDI 标准进行描述，推荐用于社会科学和教育数据。
- 详细信息请参考 [DDI 官方网站](https://ddialliance.org/)。
- **引用**: 在使用该数据集时，请引用该文件，并确保遵循开放数据许可协议。

---

## 数据分析与可视化

### 1. 教育程度与工资的关系
为了更好地理解数据的特征，我们展示了 **教育程度与工资的关系** 散点图：

![](python%20code.png)
![](python%20results.png)


---

## ORCID 和 DOI 信息
- **ORCID ID**: [0009-0003-2519-6097](https://orcid.org/0009-0003-2519-6097)
- **DOI**: DOI not available yet

---

## 创建过程中遇到的挑战和解决方法

### 1. 选择元数据标准
我选择了 **DDI** 标准，首先在上课的时候我们就学习了如下的几个优点：
1、Generate interactive codebooks
2、Implement data catalogues and portals
3、Transfer data between analysis packages
4、Build question banks
5、Create concordance mappings
6、Harmonize and compare data
7、Manage longitudinal data sets
同时在相关参考网站中，我也深刻意识到了以下几个**DDI** 标准的优势：
专为社会科学数据设计：DDI 标准是专门为社会科学、行为数据和经济数据设计的。因为我们的数据集涉及个人工资、年龄、婚姻状况、种族、教育程度等社会经济因素，DDI 是最适合的标准。它能够准确描述这些变量并提供详细的元数据。
全面的变量描述能力：DDI 能够帮助我们详细描述每个变量的定义、测量单位、允许的取值等信息。这一点对社会科学数据特别重要，因为研究人员通常需要在不同项目中对比和整合数据。
提升数据透明度：通过使用 DDI 标准，研究人员和其他数据用户可以更清晰地理解数据的来源、结构和使用限制，这有助于提高数据的透明度和可信度。同时，标准化的元数据能够帮助用户更快上手并使用数据，促进科学研究的开展。
因此使用 **DDI** 标准。

### 2. 使用模板和软件
在创建 ReadMe 文件和元数据文档时，我使用了多种工具和模板，具体如下：
PDF 模板：在这个任务的最开始我用PDF制作了相关图片以增强美观性，也让整个项目的主题更加清晰可见。
GitHub 模板：在文档的结构上，我参考了 GitHub 社区中常用的一些开源 ReadMe 模板。这些模板为文档提供了标准的结构，例如项目简介、数据集描述、徽章展示等。这些模板为我提供了一个清晰的框架，使得 ReadMe 文件更加规范易读。我根据项目的需求调整了这些模板，添加了数据分析和可视化部分，以适应本次项目研究。
Python 数据可视化工具：在生成数据分析的图表时，我使用了 Python 的 Matplotlib 库。我使用它生成了数据集中的 教育程度与工资的关系的柱状 图。生成的图表通过 Markdown 嵌入到了 ReadMe 文档中，帮助用户直观地理解数据分析结果。
数据管理工具：在处理数据和生成元数据文档时，我使用了 Pandas 进行数据整理和描述。通过它，我能够轻松提取数据的结构化信息，并将这些信息编写到元数据文档中。
在创建文档时，我申请并使用了我的 Open Researcher and Contributor ID (ORCID)。在文档中，我添加了 ORCID 以确保文档的作者身份明确，也为未来的研究引用提供方便。
我的 ORCID ID 是：0009-0003-2519-6097。
DOI (Digital Object Identifier)，由于数据集尚未正式发布，因此还没有生成 DOI。但一旦数据集公开，我计划为其生成 DOI 以便更方便地引用和共享。

### 3. 困难与如何克服困难
1. 不熟悉Github软件
在最开始时，我对 ReadMe 文件一无所知，我在浏览了推荐的视频后也是一头雾水，我看到了视频里面提到的Github软件，于是我开始对Github进行了进一步探索，这对于没有用过这类型软件的我来说是一个漫长的过程，我需要一步步去阅读去浏览我到底要做什么。但是好在互联网上面的资源足够丰富，我也对Github的使用有了进一步了解。

2. 难以形成软件之间的链接
其实我之前已经用了python等相关软件对上面Wage这个文件进行过了一些分析，我希望能够把分析结果放在Readme文件里面，但是我发现这个过程非常困难。我制作了一些图片，来让数据更加可视化，但是我不知道如何让他体现在Readme里面，即使我成功的使用Github让图片可以展示，但是单独的Readme文件又无法正常浏览图片，我尝试了很多办法，最后还是从网络上和在AI软件的帮助下成功的让我的Readme文件上呈现了我希望的内容。

3. 数据描述的准确性和完整性
在撰写数据集描述时，我发现需要提供详细的元数据和数据字典，这对我来说非常困难。尤其是当需要解释每个变量的含义、数据格式和取值范围和数据字典编辑时，都给我带来的巨大的困扰，于是我尝试结合一些较为熟悉的数据统计或是数据分析软件，例如Python来帮助我进行数据描述来降低错误的发生。





---
