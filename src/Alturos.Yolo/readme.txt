Thanks for use the Alturos.Yolo package

This package delivers all dependencies for cpu detection.

If you need gpu detection please install cuda and cudnn.
And copy the cudnn64_7.dll in the x64 directory.
If all the dependencies are available Alturos.Yolo automatically switches to gpu mode.

For an easy start please install-package Alturos.YoloV2TinyVocData

Example:

var configurationDetector = new ConfigurationDetector();
var config = configurationDetector.Detect();

using (var yoloWrapper = new YoloWrapper(config))
{
	var result = yoloWrapper.Detect(@"image.jpg");
}
