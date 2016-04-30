# MatConvNet-Calvin

**MatConvNet-Calvin** is a wrapper around MatConvNet that (re-)implements
several state of-the-art papers in object detection and semantic segmentation.
Calvin is a Computer Vision research group at the University of Edinburgh (http://calvin.inf.ed.ac.uk/).
Copyrights by Holger Caesar and Jasper Uijlings, 2015-2016.

**Implementations:**
- **Fast R-CNN** by Girshick et al.
  (http://arxiv.org/abs/1504.08083)
  (incl. bounding box regression, ROI pooling)
- **End-to-end region based semantic segmentation** by Caesar et al.
  (TBD)
  (incl. freeform ROI pooling, region-to-pixel layer)
- **Fully Convolutional Networks for Semantic Segmentation** by Long et al.
  (http://arxiv.org/abs/1411.4038)
  (based on matconvnet-fcn, extended for arbitrary classes)
  (https://github.com/vlfeat/matconvnet-fcn)
- **Fully Convolutional Multi-Class Multipe Instance Learning** by Pathak et al.
  (http://arxiv.org/abs/1412.7144)
  (based on matconvnet-fcn and a modified loss using the SegmentationLabelPresence layer)

**Installation:**
- Install Matlab
- Clone the repository "git clone --recursive https://github.com/nightrome/matconvnet-calvin.git"
- Setup MatConvNet
  - cd matconvnet/matlab;
  - vl_compilenn('EnableGpu', true);
  - vl_setupnn();
  - cd ../..;
- Setup MatConvNet-Calvin
  - cd matconvnet-calvin/matlab;
  - vl_compilenn_calvin();
  - vl_setupnn_calvin();
  - cd ../..;
- For missing files please contact the authors

**Dependencies:**
- **MatConvNet**: beta18 (http://github.com/vlfeat/matconvnet).
- **MatConvNet-FCN**: (http://github.com/vlfeat/matconvnet-fcn)
