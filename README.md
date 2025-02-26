# Bad Apple (but it's an AI image generator)

## Overview
This project is a perpetuation of the running gag surrounding the [Bad Apple music video](URL "[https://en.wikipedia.org/wiki/ImageNet](https://www.youtube.com/watch?v=FtutLA63Cp8)"). Every frame in the video was taught to a custom deep neural network image Generator/Decoder. Takes an input number (0 to 6571) to generate the associated image frame from the music video. 

## How-to
1. Install required dependencies
2. Run the Bad-Apple-Demo.ipynb in your python notebook editor (such as jupyterlab)

## File Structure
- `models/`: Contains pretrained model objects. Conv_Decoder_Clean.pkl is the default version, Conv_Decoder_Crunchy.pkl is a visually interesting version that preserves some visual artifacts from training
- `video_frames/`: Contains 6572 image frames extracted from the video.
- `Bad-Apple-Demo.ipynb`: Demo file which you can run to generate the images. Automatically inputs numbers 0 to 6571, and the model automatically generates the corresponding images sequentially.
- `BadApple.mp3`: Contains audio for Bad Apple. Can be run simultaneously when generating images, but usually isn't synced with the render speed of the model.
- `BadApple.mp4`: Contains the [Bad Apple music video](URL "[https://en.wikipedia.org/wiki/ImageNet](https://www.youtube.com/watch?v=FtutLA63Cp8)").
- `LICENSE`: License.
- `README.md`: Documentation.
- `model-training.ipynb`: Contains final deep learning image decoder/generator architecture, optimization, configuration and hyperparameters. The hyperparameters and trainign configuration were changed many times during training to achieve a cleaner output, so the results may not be fully reproducible.
- `preprocessing.ipynb`: Preprocessing steps used to extract images and sound from the original video.

## Dependencies for running Bad-Apple-Demo.ipynb :
- Pytorch
- matplotlib
- IPython.display (typically included with Jupyter)

## License
This project is licensed under the [MIT License](LICENSE).
