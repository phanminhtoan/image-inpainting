# Source code is structurized from
- https://github.com/JiahuiYu/neuralgym
- https://github.com/JiahuiYu/generative_inpainting

This source above written with tensorflow 1.x

# Now it have been migrated to tensorflow 2.x
We can run souce code with env installed tensorflow 2.x
- Install requirement: cmd: pip install -r requirements.txt
- Install neuralgym package: this package have already migrated to tensorflow 2.x
- cmd: git clone https://github.com/phanminhtoan/neuralgym.git
- cmd: cd neuralgym
- cmd: python setup.py install

We can run project with two model

Inpainting for Face:
- cmd: python inpainting_face.py --image demo_face/case1_input.png --mask demo_face/case1_mask.png
- Result will be store in root folder: result.png

Inpainting for Place:
- cmd: python inpainting_place.py --image demo_place/case3_input.png --mask demo_place/case3_mask.png
- Result will be store in root folder: result.png

# Video demo is also add in google drive: https://drive.google.com/drive/folders/16HR0iH4SvXaCDLIyg_vNZJ42DSxu9Pi1?usp=sharing


## Please noted that when you run and got the issue as below:

dist-packages/tensorflow/python/training/py_checkpoint_reader.py", line 70, in get_tensor self, compat.as_bytes(tensor_str))

IndexError: Read less bytes than requested

### -> The reason is the model is commit with git LFS, that mean you have not been cloned comepleted this file together with source code, so that you download directly raw file update for model as link:

https://github.com/phanminhtoan/image-inpainting/raw/master/model_logs/release_places2_256/snap-0.data-00000-of-00001

https://github.com/phanminhtoan/image-inpainting/raw/master/model_logs/release_places2_256/snap-0.meta

And Update this file above in model_logs/release_places2_256

https://github.com/phanminhtoan/image-inpainting/raw/master/model_logs/release_celeba_hq_256/snap-0.data-00000-of-00001

https://github.com/phanminhtoan/image-inpainting/raw/master/model_logs/release_celeba_hq_256/snap-0.meta

And Update this file above in model_logs/release_celeba_hq_256


