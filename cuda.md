# CUDA + Tensorflow Ubuntu installation guide

1. Update Ubuntu
2. Purge nvidia and cuda
3. Install CUDA - https://developer.nvidia.com/cuda-toolkit-archive (easiest way is runfile)
4. Add cuda installation path to `LD_LIBRARY_PATH`

```
export LD_LIBRARY_PATH="/usr/local/cuda/lib64:$LD_LIBRARY_PATH"
```

5. Install cudNN library - https://developer.nvidia.com/rdp/cudnn-download (just decompress files and move to `/usr/local/cuda`)
6. Install Tensorflow - https://www.tensorflow.org/install/install_linux
7. ???
8. Test installation

```
import tensorflow as tf
hello = tf.constant('Hello, TensorFlow!')
sess = tf.Session()
print(sess.run(hello))
```

9. Profit