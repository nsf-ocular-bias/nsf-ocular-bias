---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "UFPR Fairness - Across Age"
subtitle: ""
type: updates
layout: single
summary: ""
author: "Sreeraj Ramachandran"
tags: []
categories: []  
date: 2022-06-01T11:35:52-05:00
draft: false
reading_time: true
profile: true

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
---

## Dataset
- Dataset includes 33,660 ocular samples from 1,122 subjects captured by 196 different mobile.

- All images were resized to224×224. the complete dataset is classified into three age-groups: namely young (18 to 39), middle-aged (40 to 59), and older adults (60 to 79).

- User recognition and gender classifier models are fine-tuned on randomly selected gender and age-group balanced subset from 780 participants. Subject-disjoint, gender and age-group-balanced subset selected from 342 subjects are used as the test set for authentication and 260 subjects (130 males and females) for gender classification.

- Age classifier models are fine-tuned on balanced subset selected from 432 subjects and evaluated on subset from 132 subjects, across 6 age-groups, namely 18−29, 30−39, 40−49, 50−59, 60−69 and 70−79.

<br>
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@4.0.0/dist/css/bootstrap.min.css" integrity="sha384-Gn5384xqQ1aoWXA+058RXPxPg6fy4IWvTNh0E263XmFcJlSAwiGgFAW/dAiS6JXm" crossorigin="anonymous">


<table class="table text-center table-mod">
<caption class="text-center">TABLE I: EER and FNMR at 0.01 and 0.1 FMR for user authentication using CNN models for Left (L), Right (R) ocular region,and their score-level fusion (L+R) for Young, Middle-Aged and Older adults evaluated on balanced version of UFPR ocular datasets.</caption>
<thead>
  <tr>
    <th class="tg-9wq8" rowspan="3">CNN<br></th>
    <th class="tg-9wq8" rowspan="3">Age-Group<br></th>
    <th class="tg-9wq8" colspan="3" rowspan="2">EER(%)&nbsp;&nbsp;</th>
    <th class="tg-9wq8" colspan="6">FNMR(%) @ FMR</th>
  </tr>
  <tr>
    <th class="tg-kyy7" colspan="3">0.01</th>
    <th class="tg-kyy7" colspan="3">0.1</th>
  </tr>
  <tr>
    <th class="tg-c3ow">L</th>
    <th class="tg-c3ow">R</th>
    <th class="tg-c3ow">L+R</th>
    <th class="tg-c3ow">L</th>
    <th class="tg-c3ow">R</th>
    <th class="tg-c3ow">L+R</th>
    <th class="tg-c3ow">L</th>
    <th class="tg-c3ow">R</th>
    <th class="tg-c3ow">L+R</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-kyy7" rowspan="3">ResNet-50</td>
    <td class="tg-abip">Young</td>
    <td class="tg-abip">8.60</td>
    <td class="tg-abip">9.52</td>
    <td class="tg-abip">9.06</td>
    <td class="tg-abip">37.63</td>
    <td class="tg-abip">35.35</td>
    <td class="tg-abip">36.49</td>
    <td class="tg-abip">53.74</td>
    <td class="tg-abip">54.03</td>
    <td class="tg-abip">53.89</td>
  </tr>
  <tr>
    <td class="tg-c3ow">Middle-Aged</td>
    <td class="tg-c3ow">8.62</td>
    <td class="tg-c3ow">9.08</td>
    <td class="tg-c3ow">8.85</td>
    <td class="tg-c3ow">30.76</td>
    <td class="tg-c3ow">25.04</td>
    <td class="tg-c3ow">27.9</td>
    <td class="tg-c3ow">52.23</td>
    <td class="tg-c3ow">48.55</td>
    <td class="tg-c3ow">50.39</td>
  </tr>
  <tr>
    <td class="tg-abip">Older</td>
    <td class="tg-abip">11.01</td>
    <td class="tg-abip">11.00</td>
    <td class="tg-abip">11.01</td>
    <td class="tg-abip">15.47</td>
    <td class="tg-abip">19.34</td>
    <td class="tg-abip">17.405</td>
    <td class="tg-abip">30.67</td>
    <td class="tg-abip">30.67</td>
    <td class="tg-abip">30.67</td>
  </tr>
  <tr>
    <td class="tg-9wq8" rowspan="3">MobileNet-V2</td>
    <td class="tg-c3ow">Young</td>
    <td class="tg-c3ow">7.75</td>
    <td class="tg-c3ow">7.32</td>
    <td class="tg-c3ow">7.54</td>
    <td class="tg-c3ow">33.21</td>
    <td class="tg-c3ow">26.11</td>
    <td class="tg-c3ow">29.66</td>
    <td class="tg-c3ow">51.61</td>
    <td class="tg-c3ow">48.28</td>
    <td class="tg-c3ow">49.95</td>
  </tr>
  <tr>
    <td class="tg-abip">Middle-Aged</td>
    <td class="tg-abip">9.08</td>
    <td class="tg-abip">8.68</td>
    <td class="tg-abip">8.88</td>
    <td class="tg-abip">29.18</td>
    <td class="tg-abip">28.14</td>
    <td class="tg-abip">28.66</td>
    <td class="tg-abip">51.17</td>
    <td class="tg-abip">51.31</td>
    <td class="tg-abip">51.24</td>
  </tr>
  <tr>
    <td class="tg-c3ow">Older</td>
    <td class="tg-c3ow">8.04</td>
    <td class="tg-c3ow">9.63</td>
    <td class="tg-c3ow">8.84</td>
    <td class="tg-c3ow">18.54</td>
    <td class="tg-c3ow">13.47</td>
    <td class="tg-c3ow">16.005</td>
    <td class="tg-c3ow">39.47</td>
    <td class="tg-c3ow">36.00</td>
    <td class="tg-c3ow">37.74</td>
  </tr>
  <tr>
    <td class="tg-kyy7" rowspan="3">ShuffleNet-V2</td>
    <td class="tg-abip">Young</td>
    <td class="tg-abip">6.93</td>
    <td class="tg-abip">6.96</td>
    <td class="tg-abip">6.95</td>
    <td class="tg-abip">37.63</td>
    <td class="tg-abip">38.09</td>
    <td class="tg-abip">37.86</td>
    <td class="tg-abip">56.44</td>
    <td class="tg-abip">56.26</td>
    <td class="tg-abip">56.35</td>
  </tr>
  <tr>
    <td class="tg-c3ow">Middle-Aged</td>
    <td class="tg-c3ow">8.32</td>
    <td class="tg-c3ow">9.25</td>
    <td class="tg-c3ow">8.79</td>
    <td class="tg-c3ow">37.38</td>
    <td class="tg-c3ow">46.07</td>
    <td class="tg-c3ow">41.73</td>
    <td class="tg-c3ow">55.08</td>
    <td class="tg-c3ow">61.10</td>
    <td class="tg-c3ow">58.09</td>
  </tr>
  <tr>
    <td class="tg-abip">Older</td>
    <td class="tg-abip">9.72</td>
    <td class="tg-abip">8.18</td>
    <td class="tg-abip">8.95</td>
    <td class="tg-abip">30.53</td>
    <td class="tg-abip">30.80</td>
    <td class="tg-abip">30.67</td>
    <td class="tg-abip">44.93</td>
    <td class="tg-abip">53.47</td>
    <td class="tg-abip">49.20</td>
  </tr>
  <tr>
    <td class="tg-9wq8" rowspan="3">EfficientNet-B0</td>
    <td class="tg-c3ow">Young</td>
    <td class="tg-c3ow">7.64</td>
    <td class="tg-c3ow">9.61</td>
    <td class="tg-c3ow">8.63</td>
    <td class="tg-c3ow">32.54</td>
    <td class="tg-c3ow">27.00</td>
    <td class="tg-c3ow">29.77</td>
    <td class="tg-c3ow">55.40</td>
    <td class="tg-c3ow">48.38</td>
    <td class="tg-c3ow">51.89</td>
  </tr>
  <tr>
    <td class="tg-abip">Middle-Aged</td>
    <td class="tg-abip">6.95</td>
    <td class="tg-abip">9.03</td>
    <td class="tg-abip">7.99</td>
    <td class="tg-abip">38.07</td>
    <td class="tg-abip">26.69</td>
    <td class="tg-abip">32.38</td>
    <td class="tg-abip">49.12</td>
    <td class="tg-abip">49.31</td>
    <td class="tg-abip">49.22</td>
  </tr>
  <tr>
    <td class="tg-c3ow">Older</td>
    <td class="tg-c3ow">9.34</td>
    <td class="tg-c3ow">12.08</td>
    <td class="tg-c3ow">10.71</td>
    <td class="tg-c3ow">20.80</td>
    <td class="tg-c3ow">23.33</td>
    <td class="tg-c3ow">22.065</td>
    <td class="tg-c3ow">39.73</td>
    <td class="tg-c3ow">41.74</td>
    <td class="tg-c3ow">40.74</td>
  </tr>
</tbody>
</table>

<br>

 
<table class="table text-center table-mod">
<caption class="text-center">TABLE II: Accuracy of CNN-based Gender Classification on Left Ocular Region among Young (18 to 39 years), Middle (40
to 59 years) and Older Adults (60 to 79 years).
</caption>
<thead>
  <tr>
    <th class="tg-amwm">CNN</th>
    <th class="tg-amwm" colspan="2">Young</th>
    <th class="tg-amwm" colspan="2">Middle-Aged</th>
    <th class="tg-amwm" colspan="2">Older</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-amwm"></td>
    <td class="tg-amwm">Male[%]</td>
    <td class="tg-amwm">Female[%]</td>
    <td class="tg-amwm">Male[%]</td>
    <td class="tg-amwm">Female[%]</td>
    <td class="tg-amwm">Male[%]</td>
    <td class="tg-amwm">Female[%]</td>
  </tr>
  <tr>
    <td class="tg-baqh">ResNet-50</td>
    <td class="tg-baqh">98.39</td>
    <td class="tg-baqh">98.19</td>
    <td class="tg-baqh">100</td>
    <td class="tg-baqh">96.67</td>
    <td class="tg-baqh">99.17</td>
    <td class="tg-baqh">98.06</td>
  </tr>
  <tr>
    <td class="tg-baqh">MobileNet-V2</td>
    <td class="tg-baqh">99.97</td>
    <td class="tg-baqh">99.9</td>
    <td class="tg-baqh">100</td>
    <td class="tg-baqh">99.7</td>
    <td class="tg-baqh">100</td>
    <td class="tg-baqh">100</td>
  </tr>
  <tr>
    <td class="tg-baqh">ShuffleNet-V2-50</td>
    <td class="tg-baqh">98.23</td>
    <td class="tg-baqh">97.57</td>
    <td class="tg-baqh">98.28</td>
    <td class="tg-baqh">97.56</td>
    <td class="tg-baqh">94.76</td>
    <td class="tg-baqh">98.89</td>
  </tr>
  <tr>
    <td class="tg-baqh">EfficientNet-B0</td>
    <td class="tg-baqh">95.89</td>
    <td class="tg-baqh">97.54</td>
    <td class="tg-baqh">98.58</td>
    <td class="tg-baqh">96.44</td>
    <td class="tg-baqh">95.23</td>
    <td class="tg-baqh">86.94</td>
  </tr>
</tbody>
</table>

<br>
<table class="table text-center table-mod">
<caption class="text-center">TABLE III: Accuracy of the CNN-based Gender Classification on Right Ocular Region among Young (18 to 39 years), Middle
(40 to 59 years) and Older Adults (60 to 79 years).</caption>
<thead>
  <tr>
    <th class="tg-7btt">CNN</th>
    <th class="tg-7btt" colspan="2">Young</th>
    <th class="tg-7btt" colspan="2">Middle-Aged</th>
    <th class="tg-7btt" colspan="2">Older</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-7btt"></td>
    <td class="tg-7btt">Male[%]</td>
    <td class="tg-7btt">Female[%]</td>
    <td class="tg-7btt">Male[%]</td>
    <td class="tg-7btt">Female[%]</td>
    <td class="tg-7btt">Male[%]</td>
    <td class="tg-7btt">Female[%]</td>
  </tr>
  <tr>
    <td class="tg-c3ow">ResNet-50</td>
    <td class="tg-c3ow">97.98</td>
    <td class="tg-c3ow">99.61</td>
    <td class="tg-c3ow">97.07</td>
    <td class="tg-c3ow">99.78</td>
    <td class="tg-c3ow">92.86</td>
    <td class="tg-c3ow">98.61</td>
  </tr>
  <tr>
    <td class="tg-c3ow">MobileNet-V2</td>
    <td class="tg-c3ow">96.84</td>
    <td class="tg-c3ow">92.35</td>
    <td class="tg-c3ow">95.86</td>
    <td class="tg-c3ow">98.66</td>
    <td class="tg-c3ow">94.76</td>
    <td class="tg-c3ow">97.5</td>
  </tr>
  <tr>
    <td class="tg-c3ow">ShuffleNet-V2-50</td>
    <td class="tg-c3ow">98.51</td>
    <td class="tg-c3ow">98.91</td>
    <td class="tg-c3ow">98.79</td>
    <td class="tg-c3ow">99.33</td>
    <td class="tg-c3ow">97.38</td>
    <td class="tg-c3ow">98.61</td>
  </tr>
  <tr>
    <td class="tg-c3ow">EfficientNet-B0</td>
    <td class="tg-c3ow">97.18</td>
    <td class="tg-c3ow">95.14</td>
    <td class="tg-c3ow">95.15</td>
    <td class="tg-c3ow">97.33</td>
    <td class="tg-c3ow">94.52</td>
    <td class="tg-c3ow">90</td>
  </tr>
</tbody>
</table>
<br>
<table class="table text-center table-mod">
<caption class="text-center">TABLE IV: Exact and 1-off accuracies of Age-group Classification for Young Adults</caption>
<thead>
  <tr>
    <th class="tg-baqh"></th>
    <th class="tg-amwm" colspan="2">Left Ocular</th>
    <th class="tg-amwm" colspan="2">Right Ocular</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-7btt">CNN</td>
    <td class="tg-7btt">Exact [%] </td>
    <td class="tg-7btt">1-off [%]</td>
    <td class="tg-amwm">Exact [%] </td>
    <td class="tg-amwm">1-off [%]</td>
  </tr>
  <tr>
    <td class="tg-c3ow">ResNet-50</td>
    <td class="tg-c3ow">46.72</td>
    <td class="tg-c3ow">93</td>
    <td class="tg-baqh">52.87</td>
    <td class="tg-baqh">93.16</td>
  </tr>
  <tr>
    <td class="tg-baqh">MobileNet-V2</td>
    <td class="tg-baqh">54.14</td>
    <td class="tg-baqh">91.78</td>
    <td class="tg-baqh">59.76</td>
    <td class="tg-baqh">94.9</td>
  </tr>
  <tr>
    <td class="tg-baqh">ShuffleNet-V2-50</td>
    <td class="tg-baqh">52.47</td>
    <td class="tg-baqh">91.16</td>
    <td class="tg-baqh">45.16</td>
    <td class="tg-baqh">85.27</td>
  </tr>
  <tr>
    <td class="tg-c3ow">EfficientNet-B0</td>
    <td class="tg-c3ow">28.225</td>
    <td class="tg-c3ow">53.195</td>
    <td class="tg-baqh">31.6</td>
    <td class="tg-baqh">62.64</td>
  </tr>
</tbody>
</table>

<br>
<table class="table text-center table-mod">
<caption class="text-center">TABLE V: Exact and 1-off accuracies of Age-group Classification for Middle-Aged Adults.</caption>
<thead>
  <tr>
    <th class="tg-baqh"></th>
    <th class="tg-amwm" colspan="2">Left Ocular</th>
    <th class="tg-amwm" colspan="2">Right Ocular</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-7btt">CNN</td>
    <td class="tg-7btt">Exact [%] </td>
    <td class="tg-7btt">1-off [%]</td>
    <td class="tg-amwm">Exact [%] </td>
    <td class="tg-amwm">1-off [%]</td>
  </tr>
  <tr>
    <td class="tg-c3ow">ResNet-50</td>
    <td class="tg-c3ow">31.61</td>
    <td class="tg-c3ow">81.73</td>
    <td class="tg-baqh">35.03</td>
    <td class="tg-baqh">78.43</td>
  </tr>
  <tr>
    <td class="tg-baqh">MobileNet-V2</td>
    <td class="tg-baqh">27.95</td>
    <td class="tg-baqh">86.35</td>
    <td class="tg-baqh">31.86</td>
    <td class="tg-baqh">72.69</td>
  </tr>
  <tr>
    <td class="tg-baqh">ShuffleNet-V2-50</td>
    <td class="tg-baqh">28.46</td>
    <td class="tg-baqh">75.2</td>
    <td class="tg-baqh">24.61</td>
    <td class="tg-baqh">47.98</td>
  </tr>
  <tr>
    <td class="tg-c3ow">EfficientNet-B0</td>
    <td class="tg-c3ow">20.93</td>
    <td class="tg-c3ow">57.86</td>
    <td class="tg-baqh">19.56</td>
    <td class="tg-baqh">55.73</td>
  </tr>
</tbody>
</table>

<br>
<table class="table text-center table-mod">
<caption class="text-center">TABLE VI: Exact and 1-off accuracies of Age-group Classification for Older Adults.</caption>
<thead>
  <tr>
    <th class="tg-baqh"></th>
    <th class="tg-amwm" colspan="2">Left Ocular</th>
    <th class="tg-amwm" colspan="2">Right Ocular</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-7btt">CNN</td>
    <td class="tg-7btt">Exact [%] </td>
    <td class="tg-7btt">1-off [%]</td>
    <td class="tg-amwm">Exact [%] </td>
    <td class="tg-amwm">1-off [%]</td>
  </tr>
  <tr>
    <td class="tg-c3ow">ResNet-50</td>
    <td class="tg-c3ow">28</td>
    <td class="tg-c3ow">82.3</td>
    <td class="tg-baqh">29.485</td>
    <td class="tg-baqh">71.43</td>
  </tr>
  <tr>
    <td class="tg-baqh">MobileNet-V2</td>
    <td class="tg-baqh">38.07</td>
    <td class="tg-baqh">79.82</td>
    <td class="tg-baqh">32.93</td>
    <td class="tg-baqh">76.65</td>
  </tr>
  <tr>
    <td class="tg-baqh">ShuffleNet-V2-50</td>
    <td class="tg-baqh">36.04</td>
    <td class="tg-baqh">89.65</td>
    <td class="tg-baqh">18.54</td>
    <td class="tg-baqh">56.85</td>
  </tr>
  <tr>
    <td class="tg-c3ow">EfficientNet-B0</td>
    <td class="tg-c3ow">4.97</td>
    <td class="tg-c3ow">32.3</td>
    <td class="tg-baqh">4.74</td>
    <td class="tg-baqh">27</td>
  </tr>
</tbody>
</table>


## References

{{< bibliography cited >}}
