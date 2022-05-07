# opencv-python4.5.5-cuda.whl-for-wsl2
Custom opencv-python wheel with cuda enabled build working in wsl2

#how I made the .whl
#export TMPDIR=/mnt/c/Users/#?#?# #if having trouble with wsl2 /tmp directory permissions or size restriction, may not be necessary


export FORCE_CUDA=1
export ENABLE_CONTRIB=1
export CMAKE_ARGS="-DWITH_FFMPEG=ON \
-DOPENCV_ENABLE_NONFREE=ON \
-DWITH_CUDA=ON \
-DWITH_CUDNN=ON \
-DOPENCV_DNN_CUDA=ON \
-DCUDA_TOOLKIT_ROOT_DIR=/usr/local/cuda-11.1/"


pip3 wheel . --verbose




#link if you want to try install
https://mega.nz/file/zL5WlTLD#BVVyDkb0I8iLSyUebA3Nlc3vWlLn6F9Vd7xjw3F9Cd8
