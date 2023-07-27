---
layout: post
title:  "Ethics of Data and Analytics"
permalink: "/posts/2023-06-2-ethics-of-data-and-analytics"
date:   2023-06-2 14:14:53 -0500
# categories: jekyll update
---


Joel Shapiro shared an insightful perspective on how <i>Advanced analytics and AI can easily lead to decisions that are considered “biased”</i>.
In a recent <a href="https://hbr.org/2023/05/when-to-give-employees-access-to-data-and-analytics#">HBR article</a> exploring the optimal time and degree to which data professionals and employers are to democratize data, he relates a cautionalry tale in the form of a case study featuring Goldman Sachs:


>Goldman Sachs ... was accused of discriminating by offering less credit on an Apple credit card to women than to men. In response, Goldman Sachs said it did not use gender in its model, only factors such as credit history and income. However, one could argue that credit history and income are correlated to gender and using those variables punishes women who tend to make less money on average and historically have had less opportunity to build credit. <mark>When using output that discriminates, decision-makers and data professionals alike need to understand how the data were generated and the interconnectedness of the data, as well as how to measure such things as differential treatment and much more</mark>.

To mitigate the harms to minority groups, we musst also prioritize fairness, accountability, and transparency in the development of algorithms and AI systems. This includes involving diverse stakeholders in decision-making processes, regularly auditing algorithms for bias, and ensuring that individuals and communities have the right to access, control, and understand the data collected about them.

<p style="text-align: center">***</p>

Henry Kissinger, Google's Eric Schmidt, and Daniel Huttenlocher further the subject of ethics in data and analytics -- specifically, in A.I. -- in their book "The Age of A.I." In the book, when they explore the concept of <i>Dataset Bias</i>, they make the case that machine learning requires substantial amounts of data without which AI cannot learn good models. In instances where there is insufficient data recorded for minority groups like racial minorities, the AI ends up with results that are poor in accuracy. A good example of an instance where insufficient data can lead to suboptimal results can be  found in facial recognition systems. These systems have often been trained with disproportionately fewer pictures of people of color. When they have to perform the task of identifying black people, then, they tend to perform poorly.

There is also the matter of coverage. Training AI does not just require large amounts of data. The data needs to be varied. Training AI with vast amounts of similar data results in neural networks that are incorrectly certain of outcomes because they have never encountered the precipitating conditions before. Consider for example, the extraordinary situation of a deer leaping in front of a self-driving car. If the A.I. has not be trained on what to do in such an instance, it is left unspecified as to what action it is to take.

Human Bias can also Transfer into A.I. Systems. An A.I. reward function can reward a series of chess moves that the encoder subjectively favors.

Bias is not only limited to A.I. technology either. Consider the pulse oximeter, a tool used to measure oxygen saturation in the blood. This tool has been known to overestimate the oxygen saturation in dark skinned individuals because it or its designers assumed that the way light skin absorbs light was 'normal.'