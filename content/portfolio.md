+++
date = "2012-08-14T16:11:58+05:30"
title = "Portfolio"
+++

Here is some of my projects.

### Personal Time Analysis Pipeline

Integrate time tracking app aTimeLogger, note taking app Evernote and Mac productivity app Alfred to easily generate self time analysis report.

This is a project based on my personal interest of GTD and time management. The main propose of this tool is to reviewing. Related tech: Python (Pandas, Matplotlib) , SQL.

[Code](https://github.com/YujiShen/TimeReport)

### Display Ads Challenge

A Kaggle data science competition to predict click through rate, using Apache Spark, Python, AWS. I choose this competition because the Spark course on edX using it as sample data.

The main job I did:

- Adapting the code from course to make it work on real data (60 million records).
- Deploying and tuning AWS cluster is also a great fun for me (I even built a minimal CentOS AMI with only 1GB).

### VizBurgh & Analysis

Explored and analyzed population history of neighborhoods in Pittsburgh, and focused on several ones to perform unsupervised learning in R.

Visualized overall Pittsburgh data and its neighborhoods data using maps and multiple plots in an interactive way by D3.js, HTML, CSS.

[Demo](https://yuji.im/portfolios/vizburgh/) | [Code](https://github.com/YujiShen/Vizburgh)

### Hashtag Search Engine

A simple offline search engine to recommend Hashtag based on user’s tweet. This is the Information Retrieval course project.

The main tasks we did are:

- Extract fields from data with Java and build index with Lucene.
- Combine the hit score from both hashtag and tweets and visualize result.

We did not change or devise our own search model and just using default in Lucene. A little optimization is using fuzzy query for partial matching.

I actually deployed this project on my VPS and can make it "run". But this tiny 512MB droplet can not return results in 5 minutes (sometimes report error...). So I just decide to not show the demo, and this implies the performance of this project need improve badly.

### This Blog

I put it at last because I think it might seem not that technical compared to others. But I really like this and it took me sometime to tune and optimize this blog:

- Using git and wrecker for version control and automatic deployment.
- Responsive design for all screen sizes and convenient navigation.
- Flexible and bilingual template for both English and Chinese.
- Minimal dependency by using pure Javascript without jQuery.
- Speed optimization by using CDN and minifying all files.
- Integrating Solarized Light color scheme, well, this is my personal taste : )