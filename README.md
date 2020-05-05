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

## 158334 steps ( images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_158334/result.npy
```

## 151137 steps ( images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_151137/result.npy
```

## 143940 steps ( images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_143940/result.npy
```

abs_rel,     sq_rel,        rms,    log_rms,     d1_all,         a1,         a2,         a3

0.1518,     1.1031,     5.6323,     0.2291,     0.0000,     0.7943,     0.9309,     0.9729


## 136743 steps ( images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200503_136743/result.npy
```

abs_rel,     sq_rel,        rms,    log_rms,     d1_all,         a1,         a2,         a3

0.1471,     1.0707,     5.7025,     0.2275,     0.0000,     0.7973,     0.9302,     0.9729

## 129546 steps ( images)

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
