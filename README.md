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

## 287880 steps ( images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_287880/result.npy
```


## 280683 steps ( images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_280683/result.npy
```

abs_rel,     sq_rel,        rms,    log_rms,     d1_all,         a1,         a2,         a3

0.1455,     1.0700,     5.7172,     0.2269,     0.0000,     0.8001,     0.9317,     0.9735

## 273486 steps ( images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_273486/result.npy
```

abs_rel,     sq_rel,        rms,    log_rms,     d1_all,         a1,         a2,         a3

0.1451,     1.0410,     5.6391,     0.2264,     0.0000,     0.8032,     0.9334,     0.9737

## 266289 steps ( images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_266289/result.npy
```

abs_rel,     sq_rel,        rms,    log_rms,     d1_all,         a1,         a2,         a3

0.1447,     1.0746,     5.6480,     0.2263,     0.0000,     0.8022,     0.9332,     0.9736

## 259092 steps ( images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_259092/result.npy
```

abs_rel,     sq_rel,        rms,    log_rms,     d1_all,         a1,         a2,         a3

0.1471,     1.0682,     5.7499,     0.2296,     0.0000,     0.7967,     0.9313,     0.9730


## 244698 steps ( images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_244698/result.npy
```

abs_rel,     sq_rel,        rms,    log_rms,     d1_all,         a1,         a2,         a3

0.1477,     1.0537,     5.6039,     0.2273,     0.0000,     0.7981,     0.9325,     0.9741

## 237501 steps ( images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_237501/result.npy
```

abs_rel,     sq_rel,        rms,    log_rms,     d1_all,         a1,         a2,         a3

0.1457,     1.0475,     5.5966,     0.2259,     0.0000,     0.8031,     0.9333,     0.9737

## 230304 steps ( images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_230304/result.npy
```

abs_rel,     sq_rel,        rms,    log_rms,     d1_all,         a1,         a2,         a3

0.1459,     1.0491,     5.6658,     0.2269,     0.0000,     0.8003,     0.9326,     0.9735

## 223107 steps ( images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_223107/result.npy
```

abs_rel,     sq_rel,        rms,    log_rms,     d1_all,         a1,         a2,         a3

0.1460,     1.0608,     5.7864,     0.2296,     0.0000,     0.7978,     0.9304,     0.9725

## 215910 steps ( images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_215910/result.npy
```

abs_rel,     sq_rel,        rms,    log_rms,     d1_all,         a1,         a2,         a3

0.1465,     1.0572,     5.4575,     0.2233,     0.0000,     0.8051,     0.9355,     0.9747

## 208713 steps (834852 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_208713/result.npy
```

abs_rel,     sq_rel,        rms,    log_rms,     d1_all,         a1,         a2,         a3

0.1471,     1.0802,     5.5619,     0.2269,     0.0000,     0.8042,     0.9332,     0.9733

## 201516 steps (806064 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_201516/result.npy
```

abs_rel,     sq_rel,        rms,    log_rms,     d1_all,         a1,         a2,         a3

0.1476,     1.0737,     5.7265,     0.2289,     0.0000,     0.7979,     0.9307,     0.9727

## 194319 steps (777276 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_194319/result.npy
```

abs_rel,     sq_rel,        rms,    log_rms,     d1_all,         a1,         a2,         a3

0.1473,     1.0665,     5.6569,     0.2285,     0.0000,     0.7992,     0.9316,     0.9725


## 187122 steps (748488 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_187122/result.npy
```

abs_rel,     sq_rel,        rms,    log_rms,     d1_all,         a1,         a2,         a3

0.1487,     1.0901,     5.5799,     0.2268,     0.0000,     0.8008,     0.9325,     0.9735

## 179925 steps (719700 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_179925/result.npy
```

abs_rel,     sq_rel,        rms,    log_rms,     d1_all,         a1,         a2,         a3

0.1478,     1.0853,     5.6545,     0.2278,     0.0000,     0.7972,     0.9313,     0.9726


## 172728 steps (690912 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_172728/result.npy
```

abs_rel,     sq_rel,        rms,    log_rms,     d1_all,         a1,         a2,         a3

0.1468,     1.0612,     5.5743,     0.2249,     0.0000,     0.8008,     0.9329,     0.9737


## 165531 steps (662124 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_165531/result.npy
```

abs_rel,     sq_rel,        rms,    log_rms,     d1_all,         a1,         a2,         a3

0.1491,     1.0661,     5.7109,     0.2300,     0.0000,     0.7947,     0.9300,     0.9723


## 158334 steps (633336 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_158334/result.npy
```

abs_rel,     sq_rel,        rms,    log_rms,     d1_all,         a1,         a2,         a3

0.1474,     1.0766,     5.7332,     0.2303,     0.0000,     0.7972,     0.9299,     0.9719

## 151137 steps (604548 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_151137/result.npy
```

abs_rel,     sq_rel,        rms,    log_rms,     d1_all,         a1,         a2,         a3

0.1491,     1.0765,     5.7960,     0.2310,     0.0000,     0.7906,     0.9283,     0.9723

## 143940 steps (575760 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_143940/result.npy
```

abs_rel,     sq_rel,        rms,    log_rms,     d1_all,         a1,         a2,         a3

0.1518,     1.1031,     5.6323,     0.2291,     0.0000,     0.7943,     0.9309,     0.9729


## 136743 steps (546972 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_136743/result.npy
```

abs_rel,     sq_rel,        rms,    log_rms,     d1_all,         a1,         a2,         a3

0.1471,     1.0707,     5.7025,     0.2275,     0.0000,     0.7973,     0.9302,     0.9729

## 129546 steps (518184 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_129546/result.npy
```

abs_rel,     sq_rel,        rms,    log_rms,     d1_all,         a1,         a2,         a3

0.1526,     1.1088,     5.6473,     0.2304,     0.0000,     0.7919,     0.9292,     0.9723

## 122349 steps (489396 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_122349/result.npy
```

abs_rel,     sq_rel,        rms,    log_rms,     d1_all,         a1,         a2,         a3

0.1517,     1.1036,     5.7870,     0.2343,     0.0000,     0.7912,     0.9263,     0.9707

## 115152 steps (460608 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_115152/result.npy
```

abs_rel,     sq_rel,        rms,    log_rms,     d1_all,         a1,         a2,         a3

0.1527,     1.1033,     5.6311,     0.2289,     0.0000,     0.7910,     0.9299,     0.9731

## 107955 steps (431820 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_107955/result.npy
```

abs_rel,     sq_rel,        rms,    log_rms,     d1_all,         a1,         a2,         a3

0.1505,     1.0821,     5.5885,     0.2280,     0.0000,     0.7950,     0.9304,     0.9728

## 100758 steps (403032 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_100758/result.npy
```

abs_rel,     sq_rel,        rms,    log_rms,     d1_all,         a1,         a2,         a3

0.1524,     1.1223,     5.6514,     0.2289,     0.0000,     0.7931,     0.9294,     0.9728

## 93561 steps (374244 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_93561/result.npy
```

abs_rel,     sq_rel,        rms,    log_rms,     d1_all,         a1,         a2,         a3

0.1547,     1.1248,     5.5405,     0.2280,     0.0000,     0.7943,     0.9304,     0.9732

## 86364 steps (345456 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_86364/result.npy
```

abs_rel,     sq_rel,        rms,    log_rms,     d1_all,         a1,         a2,         a3

0.1572,     1.1392,     5.8336,     0.2362,     0.0000,     0.7810,     0.9243,     0.9714

## 79167 steps (316668 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_79167/result.npy
```

abs_rel,     sq_rel,        rms,    log_rms,     d1_all,         a1,         a2,         a3

0.1561,     1.1193,     5.7139,     0.2312,     0.0000,     0.7842,     0.9264,     0.9725


## 71970 steps (287880 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_71970/result.npy
```

abs_rel,     sq_rel,        rms,    log_rms,     d1_all,         a1,         a2,         a3

0.1559,     1.1229,     5.7629,     0.2333,     0.0000,     0.7821,     0.9252,     0.9719




## 64773 steps (259092 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_64773/result.npy
```

abs_rel,     sq_rel,        rms,    log_rms,     d1_all,         a1,         a2,         a3

0.1570,     1.1204,     5.7109,     0.2334,     0.0000,     0.7819,     0.9250,     0.9717

## 57576 steps (230304 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_57576/result.npy
```

abs_rel,     sq_rel,        rms,    log_rms,     d1_all,         a1,         a2,         a3

0.1613,     1.1766,     5.9609,     0.2408,     0.0000,     0.7688,     0.9185,     0.9700

## 50379 steps (201516 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_50379/result.npy
```

abs_rel,     sq_rel,        rms,    log_rms,     d1_all,         a1,         a2,         a3

0.1589,     1.1594,     6.0337,     0.2386,     0.0000,     0.7739,     0.9191,     0.9699

## 43182 steps (172728 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_43182/result.npy
```

abs_rel,     sq_rel,        rms,    log_rms,     d1_all,         a1,         a2,         a3

0.1638,     1.1811,     6.0069,     0.2422,     0.0000,     0.7646,     0.9155,     0.9697

## 35985 steps (143940 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200502_35985/result.npy
```

abs_rel,     sq_rel,        rms,    log_rms,     d1_all,         a1,         a2,         a3
 
0.1660,     1.2168,     6.2349,     0.2474,     0.0000,     0.7534,     0.9127,     0.9694
 
 ## 28788 steps (115152 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200502_28788/result.npy
```

abs_rel,     sq_rel,        rms,    log_rms,     d1_all,         a1,         a2,         a3

0.1748,     1.2686,     6.3639,     0.2535,     0.0000,     0.7395,     0.9070,     0.9674
 
 ## 21591 steps (86364 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200502_21591/result.npy
```

abs_rel,     sq_rel,        rms,    log_rms,     d1_all,         a1,         a2,         a3

0.1773,     1.2921,     6.0127,     0.2512,     0.0000,     0.7444,     0.9081,     0.9666
 
 ## 14394 steps (57576 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200502_14394/result.npy
```

abs_rel,     sq_rel,        rms,    log_rms,     d1_all,         a1,         a2,         a3

0.2047,     1.5268,     6.8447,     0.2841,     0.0000,     0.6737,     0.8820,     0.9576
 
 ## 7197 steps (28788 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200502_7197/result.npy
```

abs_rel,     sq_rel,        rms,    log_rms,     d1_all,         a1,         a2,         a3

0.2190,     1.5843,     6.5901,     0.2852,     0.0000,     0.6564,     0.8805,     0.9577
