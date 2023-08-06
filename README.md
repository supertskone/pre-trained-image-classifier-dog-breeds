# Image Classification with Uploaded Images

Test your program's image classification capabilities by adding your own images.

### Upload and Classify Images

Ensure your `check_images.py` program can successfully classify the 40 images from the `pet_images` folder. For further testing, follow these steps:

1. Upload 4 images to the `uploaded_images` folder.
2. Run the `run_models_batch_uploaded.sh` file to classify the 4 uploaded images.

### Preparing Images for Classification

Before uploading the images, make sure they meet the following requirements:

- Images are in JPEG format with the extension `.jpg`.
- Images are approximately square, with the height and width having roughly the same number of pixels.

### Find or Capture the Following Images:

1. Dog Image - Name it `Dog_01.jpg`. Remember to note the breed of the dog in the image.
2. Pet or Animal Image (not a dog) - Name it `Animal_Name_01.jpg`, where `Animal_Name` represents the name of the animal in the picture. Use underscores to separate words if needed. For example:
   - Image of a Black Bear should be named `Black_bear_01.jpg`.
   - Image of a Frog should be named `Frog_01.jpg`.

3. Image of something that's not an animal - Name it `Object_Name_01.jpg`, where `Object_Name` indicates the object in the picture. Again, use underscores to separate words if necessary. For example:
   - Image of a Coffee Mug should be named `Coffee_mug_01.jpg`.
   - Image of a Bucket should be named `Bucket_01.jpg`.

4. Create a fourth Image of a Dog using `Dog_01.jpg`.
5. To create `Dog_02.jpg`, horizontally flip `Dog_01.jpg`. This means `Dog_02.jpg` will be a mirror image of `Dog_01.jpg`. If you encounter difficulties with the horizontal flip, you can simply rotate `Dog_01.jpg` by 180 degrees to obtain an upside-down version named `Dog_02.jpg`.

### Uploading Images

Upload all four images to the `uploaded_images` folder in the Project Workspace:

1. Double-click on the `uploaded_images` folder within the Project Workspace - Uploaded.
2. Click on the white + symbol above `/>home>workspace>uploaded_images` text.
3. Select "Upload File" from the dropdown menu.
4. Choose one of the four files and click the "Open" button.
5. Repeat the process to upload the remaining three files.

To return to the workspace folder, click on the white < symbol above `/>home>workspace>uploaded_images` text.

### Running Image Classification

Now that you have coded `check_images.py`, you can run it on all 3 models to classify the four images in the `uploaded_images` folder. Use the following shell script, which will generate the corresponding results files:

- `resnet_uploaded-images.txt`: Results using CNN model architecture ResNet.
- `alexnet_uploaded-images.txt`: Results using CNN model architecture AlexNet.
- `vgg_uploaded-images.txt`: Results using CNN model architecture VGG.

To execute the script, open a terminal window within the Project Workspace - Uploaded Images and type the following:

```bash
sh run_models_batch_uploaded.sh
```

This command will run `check_images.py` using all three model architectures to classify the four images in the `uploaded_images` folder and output their results files into the workspace.
