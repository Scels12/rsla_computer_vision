## Getting started 
How to Train YOLOv7 on a Custom Dataset
Step 1: Creating project
Before you start, you need to create a Roboflow account. Once you do that, you can create a new project in the Roboflow dashboard. Keep in mind to choose the right project type. In our case, Object Detection.
![(https://camo.githubusercontent.com/7264a275db6473f8432239dce3b8e1819208b5421d40654afce57680d6fd3311/68747470733a2f2f6d656469612e726f626f666c6f772e636f6d2f707265706172696e672d637573746f6d2d646174617365742d6578616d706c652f6372656174696e672d70726f6a6563742e6769663f696b2d73646b2d76657273696f6e3d6a6176617363726970742d312e342e33267570646174656441743d31363732393239373939383532)

Step 2: Uploading images
Next, add the data to your newly created project. You can do it via API or through our web interface.

If you drag and drop a directory with a dataset in a supported format, the Roboflow dashboard will automatically read the images and annotations together.


Step 3: Labeling
If you only have images, you can label them in Roboflow Annotate.


Step 4: Generate new dataset version
Now that we have our images and annotations added, we can Generate a Dataset Version. When Generating a Version, you may elect to add preprocessing and augmentations. This step is completely optional, however, it can allow you to significantly improve the robustness of your model.


Step 5: Exporting dataset
Once the dataset version is generated, we have a hosted dataset we can load directly into our notebook for easy training. Click Export and select the YOLO v5 PyTorch dataset format.
![](https://camo.githubusercontent.com/bda73b306551a545469d21838128066bb42d3e9cf403b756aac2620ed90a840c/68747470733a2f2f6d656469612e726f626f666c6f772e636f6d2f707265706172696e672d637573746f6d2d646174617365742d6578616d706c652f6578706f72742e6769663f696b2d73646b2d76657273696f6e3d6a6176617363726970742d312e342e33267570646174656441743d31363732393433333133373039)

