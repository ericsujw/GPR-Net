# [CVPRW 2023] GPR-Net: Multi-View Layout Estimation via a Geometry-Aware Panorama Registration Network
### [[Paper](https://openaccess.thecvf.com/content/CVPR2023W/OmniCV/html/Su_GPR-Net_Multi-View_Layout_Estimation_via_a_Geometry-Aware_Panorama_Registration_Network_CVPRW_2023_paper.html)]

We present a room layout estimation framework that jointly learns wide baseline panorama registration and layout estimation given a pair of 360 panoramas. To effectively tackle the wide baseline registration problem, we introduce a novel end-to-end supervised Geometry-aware Panorama Registration Network or GPR-Net that exploits the layout geometry and computes fine-grained correspondences on the layout boundary, instead of the global pixel-space. GPR-Net consists of two main parts. The geometry transformer learns a set of 1D horizon features sampled on the panorama. These 1D feature maps encode geometric cues describing the ceiling-wall and floor-wall layout boundaries, and the correspondence and co-visibility between layout boundaries. These learned geometric cues are further used for direct regression of relative pose (translation and rotation) with a pose transformer. The final layout is then obtained by registering the two layouts using the estimated pose and taking the union of the two individual layouts derived from the estimated layout boundary maps. Experimental results indicate that our method achieves state-of-the-art performance in both panorama registration and layout estimation on a large-scale indoor panorama dataset ZInD. Our code is available online.
