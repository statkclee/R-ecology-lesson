---
layout: lesson
root: .
lastupdated: March 21, 2016
contributors: ["Sarah Supp", "John Blischak","Gavin Simpson","Tracy Teal","Greg Wilson","Diego Barneche"," Stephen Turner","Francois Michonneau"]
maintainers: ["Francois Michonneau", "Auriel Fournier"]
domain: Ecology
topic: R for data analysis
software: R
dataurl: http://dx.doi.org/10.6084/m9.figshare.1314459
status: Teaching
---

# 데이터 카펜트리 -- R [^r-ecology]

[^r-ecology]: [Data Carpentry R for data analysis for Ecology](http://www.datacarpentry.org/R-ecology-lesson/)

데이터 카펜트리 목표는 과학기술 연구원들에게 데이터로 작업하는데 필요한 
기본적인 개념, 기술, 도구사용법을 전수해서, 연구원들이
더 빠른 시간내, 더 적은 고통으로, 더 많은 것을 수행하게 한다.
다음 학습교재는 [Data Carpentry R for data analysis for Ecology](http://www.datacarpentry.org/R-ecology-lesson/)을 
번역한 것이다.

프로그래밍 경험이 전혀 없는 워크샵 참석자를 대상으로 R 언어에 대한 소개가 되어 있다.
학습분량은 3/4일치에 해당된다. R 구문, RStudio 사용법, CSV 파일 불러오는 방법,
데이터프레임 구조, 요인 처리방법, 행과 열 추가/삭제, 각 수준별 요약 통계량 계산법,
시각화에 대한 매우 간단한 소개로 구성된다.

**R 교안 기여자 : {{page.contributors | join: ', ' %}}**

**R 교안 유지보수 담당자: {{page.maintainers | join: ', ' %}}**

**R 교안 한국어 번역: 이광춘**

**학습교안 상태: {{ page.status }}**

<!--
  [Information on Lesson Status Categories]()
-->

<!-- ###### INDEX OF LESSONS ON THIS TOPIC ###### -->

## 학습교재:

|       영문                      |                국문                  |
|---------------------------------|--------------------------------------|
| 1. [Lesson 00 Before we start](00-before-we-start.html)                       | 1. [00. 시작전](kr/00-before-we-start.html)|
| 2. [Lesson 01 Introduction to R](01-intro-to-R.html)                          | 2. [01. R 소개](kr/01-intro-to-R.html)|
| 3. [Lesson 02 Starting with data](02-starting-with-data.html)                 | 3. [02. 데이터를 갖고 출발](kr/02-starting-with-data.html)|
| 4. [Lesson 03 Introducing `data.frame`](03-data-frames.html)                  | 4. [03. `data.frame` 소개](kr/03-data-frames.html)|
| 5. [Lesson 04 Aggregating and analyzing data with dplyr](04-dplyr.html)       | 5. [04. `dplyr`로 데이터 총합과 분석](kr/04-dplyr.html)|
| 6. [Lesson 05 Data visualization with ggplot2](05-visualization-ggplot2.html) | 6. [05. `ggplot2`로 데이터 시각화](kr/05-visualization-ggplot2.html)|
| 7. [Lesson 06 R and SQL](06-r-and-sql.html)                                   | 7. [06. R 과 SQL](kr/06-r-and-sql.html)|

## 데이터

학습에 사용되는 데이터는 [{{page.dataurl %}}]({{page.dataurl %}}) 사이트에서 다운로드 받아 둔다.

특히, *\*.csv* (콤마 구분값, Comma Separated Value, CSV) 파일을 준비: *species.csv*, *plots.csv*, *surveys.csv*, and *combined.csv*.

### 사전 준비물

데이터 카펜트리는 직접 키보드에 손을 올려 실습하는 것으로 워크샵 참석자분들이 
직접 본인 컴퓨터(노트북)를 자져와서 효율적인 작업흐름이 되도록 적절한 도구를 설정해서 준비해 와야 된다.
*이번 학습과정에 사전 기술과 도구사용법에 대한 지식이 전혀 없다고 가정한다.*
하지만, 아래에 기술된 소프트웨어에 대한 사본을 컴퓨터에 준비하는 것은 필요하다.
학습교재를 워크샵에서 최대한 효과적으로 활용하기 위해서 수업 *전에* 
모든 것이 제대로 설치되어 준비되었는지 확인하면 좋다.

{% if page.software == "Python" %}
{% include pythonSetup.html %}
{% elsif page.software == "Spreadsheets" %}
{% include spreadsheetSetup.html %}
{% elsif page.software == "R" %}
{% include rSetup.html %}
{% else %}
{% include anySetup.html %}
{% endif %}

<p><strong>트위터</strong>: @datacarpentry</p>
