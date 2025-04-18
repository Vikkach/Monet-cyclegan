# Monet CycleGAN

This project uses a CycleGAN to translate real-world photos into Monet-style paintings.

## Dataset

The dataset used for this project is the "Monet CycleGAN" dataset from Kaggle. It consists of:

* monet_jpg - 300 Monet paintings sized 256x256 in JPEG format
* monet_tfrec - 300 Monet paintings sized 256x256 in TFRecord format
* photo_jpg - 7028 photos sized 256x256 in JPEG format
* photo_tfrec - 7028 photos sized 256x256 in TFRecord format

## Model

The model used in this project is a CycleGAN, which consists of two generators and two discriminators. The generators are used to translate images between the two domains (photos and Monet paintings), while the discriminators are used to distinguish between real and generated images.

## Training

The model was trained using the Adam optimizer with a learning rate of 2e-4. The training process took approximately 40 epochs.

## Results

The model was able to generate realistic Monet-style paintings from real-world photos. The generated images exhibit many of the characteristics of Monet's style, such as soft colors, blended textures, and painterly strokes.

## Usage

To use the model, simply run the `generate_images` function with a test input image. The function will return a translated image in the Monet style.

## Future Work

Future work on this project could include:

* Switching to a ResNet-based generator for more stylized results.
* Applying style-guided augmentation or content masks for fine-grained control.
* Using perceptual loss for better high-level feature alignment.
