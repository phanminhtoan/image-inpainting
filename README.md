# Source code is structurized from
- https://github.com/JiahuiYu/neuralgym
- https://github.com/JiahuiYu/generative_inpainting

This source above written with tensorflow 1.x

# Now it have been migrated to tensorflow 2.x
We can run souce code with env installed tensorflow 2.x
- Install requirement: cmd: pip install -r requirements.txt
Install neralgym package: this package have already migrated to tensorflow 2.x
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
