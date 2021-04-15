The Torchio library allows us to create patches - this is why I chose to use the Torchio library - as the patches are randomly sampled therefore we get many images from one. However we do need to be careful with patch size:

* If we use a high resolution image (ie. using the TIFF files directly and creating patches from these) and our patch size is quite small (ie. 256x256) and we choose to always have some of the positive labels (`1`) in each sample, the system will learn to say every pixel is `1` as the high resolution positives dominate the patch size
* 
