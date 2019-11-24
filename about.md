---
layout: page
permalink: /about/index.html
title: KIM GI HYUN
tags: [Gihyun, Kim, gihyun1019]
imagefeature: Gihyun.jpg
chart: true
---

<figure>
	<img src="{{ site.url }}/images/Gihyun.jpg">
	<figcaption>Kim Gi Hyun</figcaption>
</figure>

{% assign total_words = 0 %}
{% assign total_readtime = 0 %}
{% assign featuredcount = 0 %}
{% assign statuscount = 0 %}

{% for post in site.posts %}
    {% assign post_words = post.content | strip_html | number_of_words %}
    {% assign readtime = post_words | append: '.0' | divided_by:200 %}
    {% assign total_words = total_words | plus: post_words %}
    {% assign total_readtime = total_readtime | plus: readtime %}
    {% if post.featured %}
    {% assign featuredcount = featuredcount | plus: 1 %}
    {% endif %}
{% endfor %}

<!--
This is my personal blog. It currently has {{ site.posts | size }} posts in {{ site.categories | size }} categories which combinedly have {{ total_words }} words, which will take an average reader ({{ site.wpm }} WPM) approximately <span class="time">{{ total_readtime }}</span> minutes to read. {% if featuredcount != 0 %}There are <a href="{{ site.url }}/featured">{{ featuredcount }} featured posts</a>, you should definitely check those out.{% endif %} The most recent post is {% for post in site.posts limit:1 %}{% if post.description %}<a href="{{ site.url }}{{ post.url }}" title="{{ post.description }}">"{{ post.title }}"</a>{% else %}<a href="{{ site.url }}{{ post.url }}" title="{{ post.description }}" title="Read more about {{ post.title }}">"{{ post.title }}"</a>{% endif %}{% endfor %} which was published on {% for post in site.posts limit:1 %}{% assign modifiedtime = post.modified | date: "%Y%m%d" %}{% assign posttime = post.date | date: "%Y%m%d" %}<time datetime="{{ post.date | date_to_xmlschema }}" class="post-time">{{ post.date | date: "%d %b %Y" }}</time>{% if post.modified %}{% if modifiedtime != posttime %} and last modified on <time datetime="{{ post.modified | date: "%Y-%m-%d" }}" itemprop="dateModified">{{ post.modified | date: "%d %b %Y" }}</time>{% endif %}{% endif %}{% endfor %}. The last commit was on {{ site.time | date: "%A, %d %b %Y" }} at {{ site.time | date: "%I:%M %p" }} [UTC](http://en.wikipedia.org/wiki/Coordinated_Universal_Time "Temps Universel Coordonné").
-->


## [INTRODUCTION]()
- Birth: January, 01, 1994
- Number: 010-5566-7527
- University: Kangwon National University(Samcheok), Department of Computer Science


## [PROJECTS]()
### 수제공예품 재료 정리 어플리케이션  - *Team project*
<sub>2019.03.11 - 08.13 </sub>
- 흔히 '핸드메이드'라고도 불리는 수제공예품들을 만드는데 필요한 재료들과 그 가격들을 알려주는 어플리케이션. 수제공예품의 종류가 굉장히 다양한 만큼 지속적인 업데이트 계획이 필요한 시스템으로 제작하였다.
- Mobile programing, Database, SQL Server, Php, Java

### 병원의 관계도 조사 - *Team project*
<sub>2018.10.24 - 11.20 </sub>
- 특정 단체를 정해 그 단체의 관계도와 구조를 파악한 다음, 제 1,2,3 정규형을 모두 만족하는 ER다이어그램과 관계도 작성.
- PPT

### 영어공부 정보 공유 어플리케이션 - *Team Project*
<sub>2019.03.14 -  </sub>
- '만들어보기'에 의미를 두어 정식으로 사용되지 않을 영어공부에 대한 정보를 공유하는 어플리케이션. 토익공부를 중점으로 책, 강의사이트에 대한 추천 게시판 위주로 제작.
(현재 마무리가 되지 않은 상태)



## [Skills]()

### Language
C, C++, Java, SQL, Mobile Programing

### Plan
Hadoop, R



## [INTEREST]()

### Big Data, Analysis





<h2>Connect</h2>
✉️ [gihyun1019@naver.com]()  
🌐 [https://github.com/gihyun1019](https://github.com/gihyun1019)

