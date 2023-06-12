# Comparing `tmp/bit-diffusion-0.0.9.tar.gz` & `tmp/bit-diffusion-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bit-diffusion-0.0.9.tar", last modified: Thu Aug 18 04:15:44 2022, max compression
+gzip compressed data, was "bit-diffusion-0.1.0.tar", last modified: Mon Jun 12 21:02:25 2023, max compression
```

## Comparing `bit-diffusion-0.0.9.tar` & `bit-diffusion-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 04:15:44.095384 bit-diffusion-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-08-18 04:15:31.000000 bit-diffusion-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      600 2022-08-18 04:15:44.095384 bit-diffusion-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2593 2022-08-18 04:15:31.000000 bit-diffusion-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 04:15:44.095384 bit-diffusion-0.0.9/bit_diffusion/
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-08-18 04:15:31.000000 bit-diffusion-0.0.9/bit_diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    23795 2022-08-18 04:15:31.000000 bit-diffusion-0.0.9/bit_diffusion/bit_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 04:15:44.095384 bit-diffusion-0.0.9/bit_diffusion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      600 2022-08-18 04:15:44.000000 bit-diffusion-0.0.9/bit_diffusion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-08-18 04:15:44.000000 bit-diffusion-0.0.9/bit_diffusion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-18 04:15:44.000000 bit-diffusion-0.0.9/bit_diffusion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-08-18 04:15:44.000000 bit-diffusion-0.0.9/bit_diffusion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-08-18 04:15:44.000000 bit-diffusion-0.0.9/bit_diffusion.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-18 04:15:44.095384 bit-diffusion-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      859 2022-08-18 04:15:31.000000 bit-diffusion-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:02:25.193903 bit-diffusion-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-12 21:02:04.000000 bit-diffusion-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-12 21:02:25.193903 bit-diffusion-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-12 21:02:04.000000 bit-diffusion-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:02:25.193903 bit-diffusion-0.1.0/bit_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-12 21:02:04.000000 bit-diffusion-0.1.0/bit_diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23613 2023-06-12 21:02:04.000000 bit-diffusion-0.1.0/bit_diffusion/bit_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:02:25.193903 bit-diffusion-0.1.0/bit_diffusion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-12 21:02:25.000000 bit-diffusion-0.1.0/bit_diffusion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-12 21:02:25.000000 bit-diffusion-0.1.0/bit_diffusion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 21:02:25.000000 bit-diffusion-0.1.0/bit_diffusion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-12 21:02:25.000000 bit-diffusion-0.1.0/bit_diffusion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-12 21:02:25.000000 bit-diffusion-0.1.0/bit_diffusion.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 21:02:25.193903 bit-diffusion-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-12 21:02:04.000000 bit-diffusion-0.1.0/setup.py
```

### Comparing `bit-diffusion-0.0.9/LICENSE` & `bit-diffusion-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bit-diffusion-0.0.9/PKG-INFO` & `bit-diffusion-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bit-diffusion
-Version: 0.0.9
+Version: 0.1.0
 Summary: Bit Diffusion - Pytorch
 Home-page: https://github.com/lucidrains/bit-diffusion
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,denoising diffusion
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bit-diffusion-0.0.9/README.md` & `bit-diffusion-0.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     dim_mults = (1, 2, 4, 8),
 ).cuda()
 
 bit_diffusion = BitDiffusion(
     model,
     image_size = 128,
     timesteps = 100,
-    sample_time_delay = 0.2,     # they found in the paper that at lower number of timesteps, a time delay during sampling of greater than 0 helps FID. as timesteps increases, this time difference can be set to 0 as it does not help
+    time_difference = 0.1,       # they found in the paper that at lower number of timesteps, a time difference during sampling of greater than 0 helps FID. as timesteps increases, this time difference can be set to 0 as it does not help
     use_ddim = True              # use ddim
 ).cuda()
 
 trainer = Trainer(
     bit_diffusion,
     '/path/to/your/data',             # path to your folder of images
     results_folder = './results',     # where to save results
```

#### html2text {}

```diff
@@ -2,16 +2,16 @@
 Diffusion, Hinton's group's attempt at discrete denoising diffusion, in Pytorch
 It seems like they missed the mark for text, but the research direction still
 seems promising. I think a clean repository will do the research community a
 lot of benefits for those branching off from here. ## Install ```bash $ pip
 install bit-diffusion ``` ## Usage ```python from bit_diffusion import Unet,
 Trainer, BitDiffusion model = Unet( dim = 32, channels = 3, dim_mults = (1, 2,
 4, 8), ).cuda() bit_diffusion = BitDiffusion( model, image_size = 128,
-timesteps = 100, sample_time_delay = 0.2, # they found in the paper that at
-lower number of timesteps, a time delay during sampling of greater than 0 helps
+timesteps = 100, time_difference = 0.1, # they found in the paper that at lower
+number of timesteps, a time difference during sampling of greater than 0 helps
 FID. as timesteps increases, this time difference can be set to 0 as it does
 not help use_ddim = True # use ddim ).cuda() trainer = Trainer( bit_diffusion,
 '/path/to/your/data', # path to your folder of images results_folder = './
 results', # where to save results num_samples = 16, # number of samples
 train_batch_size = 4, # training batch size gradient_accumulate_every = 4, #
 gradient accumulation train_lr = 1e-4, # learning rate save_and_sample_every =
 1000, # how often to save and sample train_num_steps = 700000, # total training
```

### Comparing `bit-diffusion-0.0.9/bit_diffusion/bit_diffusion.py` & `bit-diffusion-0.1.0/bit_diffusion/bit_diffusion.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import math
 from pathlib import Path
-from random import random
 from functools import partial
 from multiprocessing import cpu_count
 
 import torch
 from torch import nn, einsum
 from torch.special import expm1
 import torch.nn.functional as F
@@ -48,22 +47,19 @@
     groups = num // divisor
     remainder = num % divisor
     arr = [divisor] * groups
     if remainder > 0:
         arr.append(remainder)
     return arr
 
-def convert_image_to(img_type, image):
-    if image.mode != img_type:
-        return image.convert(img_type)
+def convert_image_to(pil_img_type, image):
+    if image.mode != pil_img_type:
+        return image.convert(pil_img_type)
     return image
 
-def l2norm(t):
-    return F.normalize(t, dim = -1)
-
 # small helper modules
 
 class Residual(nn.Module):
     def __init__(self, fn):
         super().__init__()
         self.fn = fn
 
@@ -192,30 +188,30 @@
         context = torch.einsum('b h d n, b h e n -> b h d e', k, v)
 
         out = torch.einsum('b h d e, b h d n -> b h e n', context, q)
         out = rearrange(out, 'b h c (x y) -> b (h c) x y', h = self.heads, x = h, y = w)
         return self.to_out(out)
 
 class Attention(nn.Module):
-    def __init__(self, dim, heads = 4, dim_head = 32, scale = 10):
+    def __init__(self, dim, heads = 4, dim_head = 32):
         super().__init__()
-        self.scale = scale
+        self.scale = dim_head ** -0.5
         self.heads = heads
         hidden_dim = dim_head * heads
         self.to_qkv = nn.Conv2d(dim, hidden_dim * 3, 1, bias = False)
         self.to_out = nn.Conv2d(hidden_dim, dim, 1)
 
     def forward(self, x):
         b, c, h, w = x.shape
         qkv = self.to_qkv(x).chunk(3, dim = 1)
         q, k, v = map(lambda t: rearrange(t, 'b (h c) x y -> b h c (x y)', h = self.heads), qkv)
 
-        q, k = map(l2norm, (q, k))
+        q = q * self.scale
 
-        sim = einsum('b h d i, b h d j -> b h i j', q, k) * self.scale
+        sim = einsum('b h d i, b h d j -> b h i j', q, k)
         attn = sim.softmax(dim = -1)
         out = einsum('b h i j, b h d j -> b h i d', attn, v)
         out = rearrange(out, 'b h (x y) d -> b (h d) x y', x = h, y = w)
         return self.to_out(out)
 
 # model
 
@@ -357,15 +353,15 @@
     """ expects bits from -1 to 1, outputs image tensor from 0 to 1 """
     device = x.device
 
     x = (x > 0).int()
     mask = 2 ** torch.arange(bits - 1, -1, -1, device = device, dtype = torch.int32)
 
     mask = rearrange(mask, 'd -> d 1 1')
-    x = rearrange(x, 'b (c d) h w -> b c d h w', d = 8)
+    x = rearrange(x, 'b (c d) h w -> b c d h w', d = bits)
     dec = reduce(x * mask, 'b c d h w -> b c h w', 'sum')
     return (dec / 255).clamp(0., 1.)
 
 # bit diffusion class
 
 def log(t, eps = 1e-20):
     return torch.log(t.clamp(min = eps))
@@ -389,73 +385,79 @@
     def __init__(
         self,
         model,
         *,
         image_size,
         timesteps = 1000,
         use_ddim = False,
-        ddim_eta = 1.,
         noise_schedule = 'cosine',
-        sample_time_delay = 0.
+        time_difference = 0.,
+        bit_scale = 1.
     ):
         super().__init__()
         self.model = model
         self.channels = self.model.channels
 
         self.image_size = image_size
 
         if noise_schedule == "linear":
             self.log_snr = beta_linear_log_snr
         elif noise_schedule == "cosine":
             self.log_snr = alpha_cosine_log_snr
         else:
             raise ValueError(f'invalid noise schedule {noise_schedule}')
 
+        self.bit_scale = bit_scale
+
         self.timesteps = timesteps
         self.use_ddim = use_ddim
-        self.ddim_eta = ddim_eta
 
         # proposed in the paper, summed to time_next
         # as a way to fix a deficiency in self-conditioning and lower FID when the number of sampling timesteps is < 400
 
-        self.sample_time_delay = sample_time_delay
+        self.time_difference = time_difference
 
     @property
     def device(self):
         return next(self.model.parameters()).device
 
     def get_sampling_timesteps(self, batch, *, device):
         times = torch.linspace(1., 0., self.timesteps + 1, device = device)
         times = repeat(times, 't -> b t', b = batch)
         times = torch.stack((times[:, :-1], times[:, 1:]), dim = 0)
         times = times.unbind(dim = -1)
         return times
 
     @torch.no_grad()
-    def ddpm_sample(self, shape):
+    def ddpm_sample(self, shape, time_difference = None):
         batch, device = shape[0], self.device
 
+        time_difference = default(time_difference, self.time_difference)
+
         time_pairs = self.get_sampling_timesteps(batch, device = device)
 
         img = torch.randn(shape, device=device)
 
         x_start = None
 
         for time, time_next in tqdm(time_pairs, desc = 'sampling loop time step', total = self.timesteps):
 
             # add the time delay
 
-            time_next = F.relu(time_next - self.sample_time_delay)
+            time_next = (time_next - self.time_difference).clamp(min = 0.)
 
             noise_cond = self.log_snr(time)
 
             # get predicted x0
 
             x_start = self.model(img, noise_cond, x_start)
-            x_start.clamp_(-1., 1.)
+
+            # clip x0
+
+            x_start.clamp_(-self.bit_scale, self.bit_scale)
 
             # get log(snr)
 
             log_snr = self.log_snr(time)
             log_snr_next = self.log_snr(time_next)
             log_snr, log_snr_next = map(partial(right_pad_dims_to, img), (log_snr, log_snr_next))
 
@@ -463,34 +465,36 @@
 
             alpha, sigma = log_snr_to_alpha_sigma(log_snr)
             alpha_next, sigma_next = log_snr_to_alpha_sigma(log_snr_next)
 
             # derive posterior mean and variance
 
             c = -expm1(log_snr - log_snr_next)
-            mean = alpha_next * (img * (1 - c) / alpha + c * x_start)
 
+            mean = alpha_next * (img * (1 - c) / alpha + c * x_start)
             variance = (sigma_next ** 2) * c
-            log_variance = log(variance, eps = 1e-20)            
+            log_variance = log(variance)
 
             # get noise
 
             noise = torch.where(
                 rearrange(time_next > 0, 'b -> b 1 1 1'),
                 torch.randn_like(img),
                 torch.zeros_like(img)
             )
 
             img = mean + (0.5 * log_variance).exp() * noise
 
         return bits_to_decimal(img)
 
     @torch.no_grad()
-    def ddim_sample(self, shape):
-        batch, device, eta = shape[0], self.device, self.ddim_eta
+    def ddim_sample(self, shape, time_difference = None):
+        batch, device = shape[0], self.device
+
+        time_difference = default(time_difference, self.time_difference)
 
         time_pairs = self.get_sampling_timesteps(batch, device = device)
 
         img = torch.randn(shape, device = device)
 
         x_start = None
 
@@ -504,38 +508,31 @@
             padded_log_snr, padded_log_snr_next = map(partial(right_pad_dims_to, img), (log_snr, log_snr_next))
 
             alpha, sigma = log_snr_to_alpha_sigma(padded_log_snr)
             alpha_next, sigma_next = log_snr_to_alpha_sigma(padded_log_snr_next)
 
             # add the time delay
 
-            times_next = F.relu(times_next - self.sample_time_delay)
+            times_next = (times_next - time_difference).clamp(min = 0.)
 
-            x_start = self.model(img, log_snr, x_start)
-
-            # get predicted noise
+            # predict x0
 
-            pred_noise = (img - alpha * x_start) / sigma.clamp(min = 1e-8)
+            x_start = self.model(img, log_snr, x_start)
 
             # clip x0
 
-            x_start.clamp_(-1., 1.)
+            x_start.clamp_(-self.bit_scale, self.bit_scale)
 
-            sigma = eta * ((1 - alpha / alpha_next) * (1 - alpha_next) / (1 - alpha)).sqrt()
-            c = ((1 - alpha_next) - sigma ** 2).sqrt()
+            # get predicted noise
 
-            noise = torch.where(
-                rearrange(times_next > 0, 'b -> b 1 1 1'),
-                torch.randn_like(img),
-                torch.zeros_like(img)
-            )
+            pred_noise = (img - alpha * x_start) / sigma.clamp(min = 1e-8)
+
+            # calculate x next
 
-            img = x_start * alpha_next.sqrt() + \
-                  c * pred_noise + \
-                  sigma * noise
+            img = x_start * alpha_next + pred_noise * sigma_next
 
         return bits_to_decimal(img)
 
     @torch.no_grad()
     def sample(self, batch_size = 16):
         image_size, channels = self.image_size, self.channels
         sample_fn = self.ddpm_sample if not self.use_ddim else self.ddim_sample
@@ -543,19 +540,19 @@
 
     def forward(self, img, *args, **kwargs):
         batch, c, h, w, device, img_size, = *img.shape, img.device, self.image_size
         assert h == img_size and w == img_size, f'height and width of image must be {img_size}'
 
         # sample random times
 
-        times = torch.zeros((batch,), device = device).float().uniform_(0, 0.999)
+        times = torch.zeros((batch,), device = device).float().uniform_(0, 1.)
 
         # convert image to bit representation
 
-        img = decimal_to_bits(img)
+        img = decimal_to_bits(img) * self.bit_scale
 
         # noise sample
 
         noise = torch.randn_like(img)
 
         noise_level = self.log_snr(times)
         padded_noise_level = right_pad_dims_to(img, noise_level)
@@ -564,15 +561,15 @@
         noised_img = alpha * img + sigma * noise
 
         # if doing self-conditioning, 50% of the time, predict x_start from current set of times
         # and condition with unet with that
         # this technique will slow down training by 25%, but seems to lower FID significantly
 
         self_cond = None
-        if random() < 0.5:
+        if torch.rand((1)) < 0.5:
             with torch.no_grad():
                 self_cond = self.model(noised_img, noise_level).detach_()
 
         # predict and take gradient step
 
         pred = self.model(noised_img, noise_level, self_cond)
 
@@ -583,22 +580,21 @@
 class Dataset(Dataset):
     def __init__(
         self,
         folder,
         image_size,
         exts = ['jpg', 'jpeg', 'png', 'tiff'],
         augment_horizontal_flip = False,
-        convert_image_to = None
+        pil_img_type = None
     ):
         super().__init__()
         self.folder = folder
         self.image_size = image_size
         self.paths = [p for ext in exts for p in Path(f'{folder}').glob(f'**/*.{ext}')]
-
-        maybe_convert_fn = partial(convert_image_to, convert_image_to) if exists(convert_image_to) else nn.Identity()
+        maybe_convert_fn = partial(convert_image_to, pil_img_type) if exists(pil_img_type) else nn.Identity()
 
         self.transform = T.Compose([
             T.Lambda(maybe_convert_fn),
             T.Resize(image_size),
             T.RandomHorizontalFlip() if augment_horizontal_flip else nn.Identity(),
             T.CenterCrop(image_size),
             T.ToTensor()
@@ -630,15 +626,15 @@
         adam_betas = (0.9, 0.99),
         save_and_sample_every = 1000,
         num_samples = 25,
         results_folder = './results',
         amp = False,
         fp16 = False,
         split_batches = True,
-        convert_image_to = None
+        pil_img_type = None
     ):
         super().__init__()
 
         self.accelerator = Accelerator(
             split_batches = split_batches,
             mixed_precision = 'fp16' if fp16 else 'no'
         )
@@ -655,15 +651,15 @@
         self.gradient_accumulate_every = gradient_accumulate_every
 
         self.train_num_steps = train_num_steps
         self.image_size = diffusion_model.image_size
 
         # dataset and dataloader
 
-        self.ds = Dataset(folder, self.image_size, augment_horizontal_flip = augment_horizontal_flip, convert_image_to = convert_image_to)
+        self.ds = Dataset(folder, self.image_size, augment_horizontal_flip = augment_horizontal_flip, convert_image_to = pil_img_type)
         dl = DataLoader(self.ds, batch_size = train_batch_size, shuffle = True, pin_memory = True, num_workers = cpu_count())
 
         dl = self.accelerator.prepare(dl)
         self.dl = cycle(dl)
 
         # optimizer
```

### Comparing `bit-diffusion-0.0.9/bit_diffusion.egg-info/PKG-INFO` & `bit-diffusion-0.1.0/bit_diffusion.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bit-diffusion
-Version: 0.0.9
+Version: 0.1.0
 Summary: Bit Diffusion - Pytorch
 Home-page: https://github.com/lucidrains/bit-diffusion
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,denoising diffusion
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bit-diffusion-0.0.9/setup.py` & `bit-diffusion-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'bit-diffusion',
   packages = find_packages(exclude=[]),
-  version = '0.0.9',
+  version = '0.1.0',
   license='MIT',
   description = 'Bit Diffusion - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/bit-diffusion',
   keywords = [
@@ -16,15 +16,15 @@
     'denoising diffusion'
   ],
   install_requires=[
     'accelerate',
     'einops',
     'ema-pytorch',
     'pillow',
-    'torch',
+    'torch>=1.12.0',
     'torchvision',
     'tqdm'
   ],
   classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Topic :: Scientific/Engineering :: Artificial Intelligence',
```

