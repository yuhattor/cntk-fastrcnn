# CNTK Web Deploy Sample

You can deploy CNTK evaluation API solution with Fast R-CNN model.

Notes:
It's necessary to prepare selective search API if you want to deploy an interactive API.
Nowadays, models trained by python can be deployed as Web API by using C#.
However, it's necessary to get ROIs value to evaluate the image.
Rois can be got by using Selective Search or the like, but we don't have good way to use it in C#.
Therefore, in this web API, you have to post with these parameters.
url : image url.
rois : rois values. The format of rois should be "0 0 0 0 0 0 ... 0". The parameter length must be match the requirement of your pre-trained model.

Thank you,
Yuki
