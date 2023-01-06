# GAN-AE-P
# Prerequisites
(i) Python 3.5+
(ii) PyTorch 0.3.0

## Acknowledgement
Thank you for providing the original code.
https://github.com/ankitAMD/Self-Attention-GAN-master_pytorch

## Usage

#### 1. Clone the repository
```bash
$ git clone https://github.com/heykeetae/Self-Attention-GAN.git
$ cd Self-Attention-GAN
```

#### 2. Install datasets (CelebA or LSUN)
```bash
$ bash download.sh CelebA
or
$ bash download.sh LSUN
```


#### 3. Train 
##### (i) Train
```bash
$ python3 main.py --batch_size 64 --imsize 64 --dataset celeb --adv_loss hinge --version sagan_celeb_testing
or
$ python3 main.py --batch_size 64 --imsize 64 --dataset lsun --adv_loss hinge --version sagan_lsun_testing
```
#### 4. Enjoy the results
```bash
$ cd samples/sagan_celeb
or
$ cd samples/sagan_lsun

```
Samples generated every 100 iterations are located. The rate of sampling could be controlled via --sample_step (ex, --sample_step 100). 
