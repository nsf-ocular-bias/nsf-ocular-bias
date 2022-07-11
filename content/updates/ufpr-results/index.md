---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "UFPR Preliminary Results"
subtitle: ""
type: updates
layout: single
summary: ""
author: "Sreeraj Ramachandran"
tags: []
categories: []  
date: 2022-02-22T11:35:52-05:00
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
The UFPR-Periocular dataset was created to obtain images in unconstrained scenarios that contain realistic noises caused by occlusion, blur, and variations in lighting, distance, and
angles. 

The gender distribution of the subjects is $(53,65\\%)$ male and
$(46,35\\%)$ female, and approximately $66\\%$ of the subjects are
under $31$ years old. In total, the dataset has images captured
from $196$ different mobile devices – the five most used device
models were: Apple iPhone 8 $(4.1\\%)$, Apple iPhone 9 $(3.1\\%)$,
Xiaomi Mi 8 Lite $(3.0\\%)$, Apple iPhone 7 $(3.0\\%)$, and Samsung
Galaxy J7 Prime $(2.7\\%)$.


## Gender Classification Results
<h4 id='cm_title' style="text-align:center"></h4>
<div class='cm_container'>
  <div id="cm_btns_model" class="btn-group-vertical cm_btns_model"></div>
  <div class="cm">
    <div id="cm_btns_tm" class="btn-group cm_btns_tm">
      <input id="cm_btns_tm_5050" type="button" value="F50M50" class="btn btn-light active"></input>
      <input id="cm_btns_tm_2575" type="button" value="F25M75" class="btn btn-light"></input>
      <input id="cm_btns_tm_7525" type="button" value="F75M25" class="btn btn-light"></input>
    </div>
    <div id='cm'></div>
  </div>
</div>

<div class="cm_container">
  <div id="gc_btns_model" class="btn-group-vertical cm_btns_model"></div>
  
  <div class="cm">
    <div id="gc_acc"></div>
  </div>
  
</div>

## Subject Verification Results
<div class="cm_container">
  <div id="tb_btns_model" class="btn-group-vertical cm_btns_model"></div>
  
  <div class="cm">
    <div id="sv_eer"></div>
  </div>
  
</div>
<div id="tb_btns_tm" class="btn-group cm_btns_tm cm_container">
    <input id="tb_btns_eer" type="button" value="EER" class="btn btn-light active"></input>
    <input id="tb_btns_auc" type="button" value="AUC" class="btn btn-light"></input>
</div>

### Subject Verification All Results Table
<div id="sv_table" class="cm_container"></div>

## Visualizations
### GradCAM
<div class="gallery_container">
  <div style="display:flex;align-items:baseline">
    <h4 style="text-align:center;width:100%">GradCAM</h4>
    <input id="viz_gradcam_avgbtn" type="button" value="Show Averaged" class="btn btn-info" data-toggle="modal" data-target=".bd-example-modal-xl"></input>
  </div>

  <div class="viz_container">
    <div id="viz_gradcam_models" class="viz_btns btn-group-vertical"></div>
    <div id="viz_gradcam" class="gallery"></div>
    <div id="viz_gradcam_class" class="viz_btns btn-group-vertical viz_class"></div>
  </div>
  <div id="viz_gradcam_opts" class="viz_opts btn-group"></div>
</div>


### Guided GradCAM
<div class="gallery_container">
  <div style="display:flex;align-items:baseline">
    <h4 style="text-align:center;width:100%">Guided GradCAM</h4>
    <input id="viz_guided_gradcam_avgbtn" type="button" value="Show Averaged" class="btn btn-info" data-toggle="modal" data-target=".bd-example-modal-xl"></input>
  </div>
  <div class="viz_container">
    <div id="viz_guided_gradcam_models" class="viz_btns btn-group-vertical"></div>
    <div id="viz_guided_gradcam" class="gallery"></div>
    <div id="viz_guided_gradcam_class" class="viz_btns btn-group-vertical viz_class"></div>
  </div>
  <div id="viz_guided_gradcam_opts" class="viz_opts btn-group"></div>
</div>

### Occlusion Sensitivity
<div class="gallery_container">
  <div style="display:flex;align-items:baseline">
    <h4 style="text-align:center;width:100%">Occlusion Sensitivity</h4>
    <input id="viz_occlusion_sensitivity_avgbtn" type="button" value="Show Averaged" class="btn btn-info" data-toggle="modal" data-target=".bd-example-modal-xl"></input>
  </div>
  <div class="viz_container">
    <div id="viz_occlusion_sensitivity_models" class="viz_btns btn-group-vertical"></div>
    <div id="viz_occlusion_sensitivity" class="gallery"></div>
    <div id="viz_occlusion_sensitivity_class" class="viz_btns btn-group-vertical viz_class"></div>
  </div>
  <div id="viz_occlusion_sensitivity_opts" class="viz_opts btn-group"></div>
</div>

### Vanilla Gradients
<div class="gallery_container">
  <div style="display:flex;align-items:baseline">
    <h4 style="text-align:center;width:100%">Vanilla Gradients</h4>
    <input id="viz_vanilla_gradients_avgbtn" type="button" value="Show Averaged" class="btn btn-info" data-toggle="modal" data-target=".bd-example-modal-xl"></input>
  </div>
  <div class="viz_container">
    <div id="viz_vanilla_gradients_models" class="viz_btns btn-group-vertical"></div>
    <div id="viz_vanilla_gradients" class="gallery"></div>
    <div id="viz_vanilla_gradients_class" class="viz_btns btn-group-vertical viz_class"></div>
  </div>
  <div id="viz_vanilla_gradients_opts" class="viz_opts btn-group"></div>
</div>

### Integrated Gradients
<div class="gallery_container">
  <div style="display:flex;align-items:baseline">
    <h4 style="text-align:center;width:100%">Integrated Gradients</h4>
    <input id="viz_integrated_gradients_avgbtn" type="button" value="Show Averaged" class="btn btn-info" data-toggle="modal" data-target=".bd-example-modal-xl"></input>
  </div>
  <div class="viz_container">
    <div id="viz_integrated_gradients_models" class="viz_btns btn-group-vertical"></div>
    <div id="viz_integrated_gradients" class="gallery"></div>
    <div id="viz_integrated_gradients_class" class="viz_btns btn-group-vertical viz_class"></div>
  </div>
  <div id="viz_integrated_gradients_opts" class="viz_opts btn-group"></div>
</div>

### SmoothGrad
<div class="gallery_container">
  <div style="display:flex;align-items:baseline">
    <h4 style="text-align:center;width:100%">SmoothGrad</h4>
    <input id="viz_smoothgrad_avgbtn" type="button" value="Show Averaged" class="btn btn-info" data-toggle="modal" data-target=".bd-example-modal-xl"></input>
  </div>
  <div class="viz_container">
    <div id="viz_smoothgrad_models" class="viz_btns btn-group-vertical"></div>
    <div id="viz_smoothgrad" class="gallery"></div>
    <div id="viz_smoothgrad_class" class="viz_btns btn-group-vertical viz_class"></div>
  </div>
  <div id="viz_smoothgrad_opts" class="viz_opts btn-group"></div>
</div>

### Gradients x Input
<div class="gallery_container">
  <div style="display:flex;align-items:baseline">
    <h4 style="text-align:center;width:100%">Gradients x Input</h4>
    <input id="viz_gradients_input_avgbtn" type="button" value="Show Averaged" class="btn btn-info" data-toggle="modal" data-target=".bd-example-modal-xl"></input>
  </div>
  <div class="viz_container">
    <div id="viz_gradients_input_models" class="viz_btns btn-group-vertical"></div>
    <div id="viz_gradients_input" class="gallery"></div>
    <div id="viz_gradients_input_class" class="viz_btns btn-group-vertical viz_class"></div>
  </div>
  <div id="viz_gradients_input_opts" class="viz_opts btn-group"></div>
</div>


<div class="modal fade bd-example-modal-xl" tabindex="-1" role="dialog" aria-labelledby="myExtraLargeModalLabel" aria-hidden="true">
  <div class="modal-dialog modal-lg">
    <div class="modal-content">
      <div class="modal-header">
        <h5 class="modal-title">Averaged Map</h5>
        <button type="button" class="close" data-dismiss="modal" aria-label="Close">
          <span aria-hidden="true">&times;</span>
        </button>
      </div>
      <img id="viz_avg_modal" src="">
    </div>
  </div>
</div>


---

## References

{{< bibliography cited >}}

<script type="module" src="ufpr.js"></script>