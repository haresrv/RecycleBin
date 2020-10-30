This PCB dataset contains 47 high quality PCB images with bounding box annotation for PCB component detection. 
In the dataset, there are 31 component types and about 60k component instances.
 Note that 3 images are removed from the dataset due to IP issues. 
 Each subfolder contains an image and an XML annotation file manually labeled using 
 labelImage(https://github.com/tzutalin/labelImg).

In the annotation file, we label the bounding box of components as well as texts following PASCAL VOC format.
 The type information can be found in object.name, while the bounding box info 
 can be found in object.bndbox in the format of (xmin, ymin, xmax, ymax).
  The names of the component bounding box are in “TYPE TEXT_LABEL” format starting with its type and 
  then the associated text label on the image. As for text bounding boxes, 
  their names are in "text TEXT_LABEL" format starting with a "text" identifier
   and ended with its actual text label on the image.
    A space is inserted in between. Th bounding box location is 
    

Please cite our paper if using this dataset:
https://arxiv.org/abs/1811.06994
@inproceedings{kuo2019data,
    title = {Data-Efficient Graph Embedding Learning for PCB Component Detection},
    author = {Kuo, Chia-Wen and Ashmore, Jacob and Huggins, David and Kira, Zsolt},
    booktitle={2019 IEEE Winter Conference on Applications of Computer Vision (WACV)},
    year = {2019},
    organization={IEEE}
}
