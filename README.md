# Sfm Learner_eval
Abs Rel Error Calculation

[Original Code](https://github.com/tinghuiz/SfMLearner)

# How to use

## 1 Make npy file from model

### Input Example

```shell
python test_kitti_depth.py --dataset_dir='/home/ubuntu/data/raw_data_KITTI/' --output_dir='/home/ubuntu/data/SfMLearner_result_20200413' --ckpt_file='/home/ubuntu/data/models_SfMLearner/model-190532'
```

If you want use checkpoint of struct2depth or depth from video, use the code [here](https://github.com/go125/TestCheckpointFromDFV).

## 2 Calculate Abs Rel Error


### Input Example for checkpoint from SfMLearner

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/SfMLearner_result_20200413/model-190532.npy
```

### Input Example for checkpoint from stuct2depth

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200430/result.npy
```

### Input Example for checkpoint from Depth from Video in the Wild

#### kitti_learned_intrinsics

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200501/result.npy
```

#### cityscapes_kitti_learned_intrinsics

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200501_2/result.npy
```

# Sekilab AWS Result

## 302274 steps (1209096 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_302274/result.npy
```


## 295077 steps (1180308 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_295077/result.npy
```



## 287880 steps (1151520 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_287880/result.npy
```




## 280683 steps (1122732 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_280683/result.npy
```



## 273486 steps (1093944 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_273486/result.npy
```



## 266289 steps (1065156 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_266289/result.npy
```



## 259092 steps (1036368 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_259092/result.npy
```



## 251895 steps (1036368 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_251895/result.npy
```




## 244698 steps (978792 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_244698/result.npy
```



## 237501 steps (950004 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_237501/result.npy
```



## 230304 steps (921216 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_230304/result.npy
```



## 223107 steps (892428 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_223107/result.npy
```



## 215910 steps (863640 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_215910/result.npy
```



## 208713 steps (834852 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_208713/result.npy
```



## 201516 steps (806064 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_201516/result.npy
```



## 194319 steps (777276 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_194319/result.npy
```




## 187122 steps (748488 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_187122/result.npy
```



## 179925 steps (719700 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_179925/result.npy
```




## 172728 steps (690912 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_172728/result.npy
```



## 165531 steps (662124 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_165531/result.npy
```




## 158334 steps (633336 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_158334/result.npy
```



## 151137 steps (604548 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_151137/result.npy
```



## 143940 steps (575760 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_143940/result.npy
```




## 136743 steps (546972 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_136743/result.npy
```



## 129546 steps (518184 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_129546/result.npy
```



## 122349 steps (489396 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_122349/result.npy
```



## 115152 steps (460608 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_115152/result.npy
```



## 107955 steps (431820 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_107955/result.npy
```



## 100758 steps (403032 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_100758/result.npy
```



## 93561 steps (374244 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_93561/result.npy
```



## 86364 steps (345456 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_86364/result.npy
```



## 79167 steps (316668 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_79167/result.npy
```




## 71970 steps (287880 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_71970/result.npy
```






## 64773 steps (259092 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200508_64773/result.npy
```


## 57576 steps (230304 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200508_57576/result.npy
```



## 50379 steps (201516 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200508_50379/result.npy
```



## 43182 steps (172728 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200508_43182/result.npy
```



## 35985 steps (143940 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200508_35985/result.npy
```


 
 ## 28788 steps (115152 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200508_28788/result.npy
```


 
 ## 21591 steps (86364 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200508_21591/result.npy
```


 
 ## 14394 steps (57576 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200508_14394/result.npy
```


 
 ## 7197 steps (28788 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200508_7197/result.npy
```


