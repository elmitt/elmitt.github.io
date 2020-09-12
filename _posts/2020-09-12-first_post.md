# Starting this blog with...embedding images in Jupyter style notebooks 

Here are a few ways I know:

## **In a markdown cell**

  1. drag&drop from your computer: 

       will create a `![]()` , which will be prefilled with:
       
        `![Imagename.extention](attachement:Imagename.extention)`

  2. using the img icon to insert URL (on a Kaggle or google Colab notebook): 

        will create the same `![]()` , which you need to insert URL in `()`. 

        > URL **MUST** have image extension (jpg, png,…).

  3. If you also need to edit image size (which isn't possible with method 1 or 2 (or @ least IDK how!)), use either of these formats:

       `<img src="attachment:imagename_from_method1.extension" width="???px">`

       `<img src="http://.../imagename_from_method2.extension" width="???px">`

## **In a code cell**

   1. Os module 
   (example from Kaggle kernel):
   
          import os
       
          from IPython.display import Image
         
          Image(filename="../input/yourdata/IMG_name.jpg", width= ???, height=???)
