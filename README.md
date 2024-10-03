
![工资及相关因素](Personal%20salary%20and%20other%20factors.png)

## 项目背景
该数据集包含了个人的工资及其相关的社会、经济因素，如年龄、婚姻状态、种族、教育程度、健康状况等。数据可用于分析哪些因素对工资水平有显著影响，特别是在“学习分析”（Learning Analytics）项目的背景下，可探索不同人群的工资差异和背后的学习、教育背景。

具体来说，研究目标包括：
- **探索教育背景对工资的长期影响**：不同教育程度的受访者在职业发展中的薪资增长情况。
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

详细信息请参考 [DDI 官方网站](https://ddialliance.org/)。

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
- **引用**: 在使用该数据集时，请引用该文件，并确保遵循开放数据许可协议。

---

## 数据分析与可视化

### 1. 教育程度与工资的关系
为了更好地理解数据的特征，我们展示了 **教育程度与工资的关系** 散点图：

![教育程度与工资的关系](education_vs_wage_plot.png)

### 2. 地区与工资的分布
下图展示了不同地区的工资分布情况：

![地区与工资的关系](region_vs_wage_plot.png)

---

## ORCID 和 DOI 信息
- **ORCID ID**: [0009-0003-2519-6097](https://orcid.org/0009-0003-2519-6097)
- **DOI**: DOI not available yet

---

## 创建过程中遇到的挑战和解决方法

### 1. 选择元数据标准
我们选择了 **DDI** 标准，因为它在社会科学领域被广泛使用，并且能够很好地支持数据集中文件、变量、采样等细节的描述。尽管 DDI 是一个强大的标准，但学习并理解其所有规范可能需要时间。通过参考官方文档和相关教程，我们克服了这一挑战。

### 2. 使用模板和软件
1. **软件选择**: 我使用了 **Typora** 来编写 Markdown 文档，因其支持 HTML 格式化和方便的实时预览功能。
2. **图表生成**: 使用 Python 和 Matplotlib 生成图表，并通过 Markdown 将图表嵌入到 ReadMe 文件中。
3. **数据字典**: 开始时对如何使用代码生成数据字典不太熟悉，通过参考视频和文档，学习了 Markdown 中创建表格的方式。

---

## 未来工作方向
未来可以进一步分析：
- **婚姻状态与工资的关系**：探索婚姻对个人工资的影响。
- **健康状况的长期影响**：分析健康状况对职业发展的长期影响，尤其是在不同种族和地区背景下。

---

