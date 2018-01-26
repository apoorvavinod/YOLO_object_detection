This is a Keras/TensorFlow implementation of the YOLO algorithm.

How to run:
1. Clone repository
2. Place your images in the 'images' folder
3. Download cfg,weights from YOLO website and convert them to Keras 	model as described below. 
3. Open the notebook and run the code.
4. output will be saved in the 'out' folder.

Converting Darknet model to Keras model: (Directly quoting Allan Zelener - YAD2K: Yet Another Darknet 2 Keras https://github.com/allanzelener/YAD2K)

1. If you're not on Linux, you may need to install 'wget'. 
	For MacOS : https://stackoverflow.com/questions/33886917/how-to-install-wget-in-macos-capitan-sierra/33902055
	For Windows: https://eternallybored.org/misc/wget/

2. Download weights from official YOLO website:
	wget http://pjreddie.com/media/files/yolo.weights

3. Load cfg and convert Darknet model to Keras model:
	wget https://raw.githubusercontent.com/pjreddie/darknet/master/cfg/yolo.cfg
	./yad2k.py yolo.cfg yolo.weights model_data/yolo.h5

Running the above cmds will save the converted model 'yolo.h5' in the 'model_data' folder.

References:

1. YOLO's official website - https://pjreddie.com/darknet/yolo/
2. 'YOLO9000: Better,Faster,Stronger'  - Joseph Redmon, Ali Farhadi
3. 'YAD2K: Yet Another Darknet 2 Keras' - Allan Zelener (https://github.com/allanzelener/YAD2K)
