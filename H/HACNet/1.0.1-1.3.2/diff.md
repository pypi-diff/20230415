# Comparing `tmp/HACNet-1.0.1.tar.gz` & `tmp/HACNet-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HACNet-1.0.1.tar", last modified: Fri Jan  6 20:12:27 2023, max compression
+gzip compressed data, was "HACNet-1.3.2.tar", last modified: Sat Apr 15 14:29:14 2023, max compression
```

## Comparing `HACNet-1.0.1.tar` & `HACNet-1.3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-01-06 20:12:27.703210 HACNet-1.0.1/
-drwxrwxrwx   0        0        0        0 2023-01-06 20:12:27.609482 HACNet-1.0.1/HACNet/
--rw-rw-rw-   0        0        0    15086 2023-01-06 20:12:11.000000 HACNet-1.0.1/HACNet/CNN.py
--rw-rw-rw-   0        0        0    15327 2023-01-06 20:12:11.000000 HACNet-1.0.1/HACNet/GCN.py
--rw-rw-rw-   0        0        0     9909 2023-01-06 20:12:11.000000 HACNet-1.0.1/HACNet/MLP.py
--rw-rw-rw-   0        0        0        2 2023-01-06 20:12:11.000000 HACNet-1.0.1/HACNet/__init__.py
--rw-rw-rw-   0        0        0    16925 2023-01-06 20:12:11.000000 HACNet-1.0.1/HACNet/functions.py
-drwxrwxrwx   0        0        0        0 2023-01-06 20:12:27.703210 HACNet-1.0.1/HACNet.egg-info/
--rw-rw-rw-   0        0        0      319 2023-01-06 20:12:26.000000 HACNet-1.0.1/HACNet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-01-06 20:12:26.000000 HACNet-1.0.1/HACNet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-06 20:12:26.000000 HACNet-1.0.1/HACNet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-01-06 20:12:26.000000 HACNet-1.0.1/HACNet.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1090 2023-01-06 20:12:11.000000 HACNet-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      319 2023-01-06 20:12:27.703210 HACNet-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3452 2023-01-06 20:12:11.000000 HACNet-1.0.1/README.md
--rw-rw-rw-   0        0        0       86 2023-01-06 20:12:27.703210 HACNet-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      444 2023-01-06 20:12:11.000000 HACNet-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 14:29:14.505100 HACNet-1.3.2/
+drwxrwxrwx   0        0        0        0 2023-04-15 14:29:14.473829 HACNet-1.3.2/HACNet/
+-rw-rw-rw-   0        0        0    14950 2023-04-15 14:28:01.000000 HACNet-1.3.2/HACNet/CNN.py
+-rw-rw-rw-   0        0        0    15340 2023-04-15 14:28:01.000000 HACNet-1.3.2/HACNet/GCN.py
+-rw-rw-rw-   0        0        0     8898 2023-04-15 14:28:01.000000 HACNet-1.3.2/HACNet/MLP.py
+-rw-rw-rw-   0        0        0        2 2023-04-15 14:28:01.000000 HACNet-1.3.2/HACNet/__init__.py
+-rw-rw-rw-   0        0        0    16922 2023-04-15 14:28:01.000000 HACNet-1.3.2/HACNet/functions.py
+drwxrwxrwx   0        0        0        0 2023-04-15 14:29:14.505100 HACNet-1.3.2/HACNet.egg-info/
+-rw-rw-rw-   0        0        0      319 2023-04-15 14:29:14.000000 HACNet-1.3.2/HACNet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-04-15 14:29:14.000000 HACNet-1.3.2/HACNet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 14:29:14.000000 HACNet-1.3.2/HACNet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-15 14:29:14.000000 HACNet-1.3.2/HACNet.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1090 2023-04-15 14:28:02.000000 HACNet-1.3.2/LICENSE
+-rw-rw-rw-   0        0        0      319 2023-04-15 14:29:14.505100 HACNet-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3536 2023-04-15 14:28:02.000000 HACNet-1.3.2/README.md
+-rw-rw-rw-   0        0        0       86 2023-04-15 14:29:14.505100 HACNet-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      444 2023-04-15 14:28:02.000000 HACNet-1.3.2/setup.py
```

### Comparing `HACNet-1.0.1/HACNet/CNN.py` & `HACNet-1.3.2/HACNet/CNN.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,14 @@
     1) checkpoint file from the endpoint of the training
     2) checkpoint file from the epoch with highest average correlation on validation
     """
 
     # define parameters
     batch_size = 50
     learning_rate = .0007
-    learning_decay_iter=150
     epoch_count = 100
 
     # set CUDA for PyTorch
     use_cuda = torch.cuda.is_available()
     device = torch.device('cuda:0')
     torch.cuda.set_device(0)
 
@@ -158,30 +157,29 @@
     val_dataloader = DataLoader(val_dataset, batch_size=batch_size, shuffle=False)
 
     # define model and helper functions
     model = CNN(use_cuda=use_cuda)
     model.to(device)
     loss_func = nn.MSELoss().float()
     optimizer = RMSprop(model.parameters(), lr=learning_rate)
-    scheduler = lr_scheduler.StepLR(optimizer, step_size=150, gamma=0.95)
     
     # initialize training variables
     epoch_start = 0
     step = 0
     epoch_train_losses, epoch_val_losses, epoch_avg_corr = [], [], []
     best_average_corr = float('-inf')
 
     #load previous checkpoint if applicable
     if previous_checkpoint!=None:
         best_checkpoint = torch.load(best_previous_checkpoint, map_location = device)
         torch.save(best_checkpoint, best_checkpoint_path)
         best_average_corr = best_checkpoint["best_avg_corr"]
         checkpoint = torch.load(previous_checkpoint, map_location=device)
         model_state_dict = checkpoint.pop('model_state_dict')
-        model.load_state_dict(model_state_dict, strict=False)
+        model.load_state_dict(model_state_dict, strict=True)
         optimizer.load_state_dict(checkpoint['optimizer_state_dict'])
         epoch_start = checkpoint['epoch'] + 1
         step=checkpoint['step']
         epoch_train_losses = checkpoint['epoch_train_losses']
         epoch_val_losses = checkpoint['epoch_val_losses']
         epoch_avg_corr = checkpoint['epoch_avg_corr']
         print('checkpoint loaded: %s' % previous_checkpoint)
@@ -235,15 +233,14 @@
             y_pred_epoch[batch_ind*batch_size:batch_ind*batch_size+bsize] = ypred_batch.cpu().float().data.numpy()[:,0]
 
         # compute loss 
             loss = loss_func(ypred_batch.cpu().float(), y_batch_cpu.float())
             optimizer.zero_grad()
             loss.backward()
             optimizer.step()
-            scheduler.step()
             step += 1
             print("[%d/%d-%d/%d] training loss: %.3f" % (epoch_ind+1, epoch_count, batch_ind+1, batch_count, loss))
 
         epoch_train_losses.append(mean_squared_error(y_true_epoch, y_pred_epoch))
         val_loss, average_corr = validate_model()
         epoch_val_losses.append(val_loss)
         epoch_avg_corr.append(average_corr)
@@ -318,15 +315,15 @@
     model.to(device)
     if isinstance(model, (DistributedDataParallel, DataParallel)):
         model = model.module
     # load checkpoint file
     checkpoint = torch.load(checkpoint_path, map_location=device)
     # model state dict
     model_state_dict = checkpoint.pop("model_state_dict")
-    model.load_state_dict(model_state_dict, strict=False)
+    model.load_state_dict(model_state_dict, strict=True)
     # create empty arrays to hold predicted and true values
     ytrue_arr = np.zeros((len(dataset),), dtype=np.float32)
     ypred_arr = np.zeros((len(dataset),), dtype=np.float32)
     flatfeat_arr = np.zeros((len(dataset), 2048 + 1))
     pdbid_arr = np.zeros((len(dataset),), dtype=object)
     pred_list = []
     model.eval()
```

### Comparing `HACNet-1.0.1/HACNet/GCN.py` & `HACNet-1.3.2/HACNet/GCN.py`

 * *Files 0% similar despite different names*

```diff
@@ -223,15 +223,15 @@
     if load_checkpoint_path != None:
         if torch.cuda.is_available():
             model_train_dict = torch.load(load_checkpoint_path)
             best_checkpoint = torch.load(best_previous_checkpoint)
         else:
             model_train_dict = torch.load(load_checkpoint_path, map_location=torch.device('cpu'))
             best_checkpoint = torch.load(best_previous_checkpoint, map_location = torch.device('cpu'))
-        model.load_state_dict(model_train_dict['model_state_dict'])
+        model.load_state_dict(model_train_dict['model_state_dict'], strict=True)
         checkpoint_epoch = model_train_dict['epoch']
         checkpoint_step = model_train_dict['step']
         epoch_train_losses = model_train_dict['epoch_train_losses']
         epoch_val_losses = model_train_dict['epoch_val_losses']
         epoch_avg_corr = model_train_dict['epoch_avg_corr']
         val_dict = model_train_dict['validate_dict']
         torch.save(best_checkpoint, best_checkpoint_path)
```

### Comparing `HACNet-1.0.1/HACNet/MLP.py` & `HACNet-1.3.2/HACNet/MLP.py`

 * *Files 9% similar despite different names*

```diff
@@ -165,15 +165,15 @@
     #load previous checkpoint if applicable
     if load_previous_checkpoint:
         best_checkpoint = torch.load(best_previous_checkpoint, map_location = device)
         best_checkpoint_dict = best_checkpoint.pop("model_state_dict")
         best_average_corr = best_checkpoint["best_avg_corr"]
         checkpoint = torch.load(previous_checkpoint, map_location=device)
         model_state_dict = checkpoint.pop("model_state_dict")
-        model.load_state_dict(model_state_dict, strict=False)
+        model.load_state_dict(model_state_dict, strict=True)
         optimizer.load_state_dict(checkpoint["optimizer_state_dict"])
         epoch_start = checkpoint["epoch"]
         loss = checkpoint["loss"]
         epoch_train_losses = checkpoint["epoch_train_losses"]
         epoch_val_losses = checkpoint["epoch_val_losses"]
         epoch_avg_corr = checkpoint["epoch_avg_corr"]
     for epoch_ind in range(epoch_start, epoch_count):
@@ -187,48 +187,30 @@
         # compute loss
             loss = loss_fn(ypred_batch.cpu().float(), y_batch_cpu.float())
             losses.append(loss.cpu().data.item())
             optimizer.zero_grad()
             loss.backward()
             optimizer.step()
             scheduler.step()
-            val_loss, average_corr = validate_model()
-            checkpoint_dict = {
-                "model_state_dict": model.state_dict(),
-                "optimizer_state_dict": optimizer.state_dict(),
-                "loss": loss,
-                "step": step,
-                "epoch": epoch_ind,
-                "epoch_val_losses": epoch_val_losses,
-                "epoch_train_losses": epoch_train_losses,
-                "epoch_avg_corr" : epoch_avg_corr,
-                "best_avg_corr" : best_average_corr 
-            }
-            if (average_corr > best_average_corr):
-                best_average_corr = average_corr
-                checkpoint_dict["best_avg_corr"] = best_average_corr
-                best_checkpoint_dict = checkpoint_dict
-                torch.save(best_checkpoint_dict, best_checkpoint_path)
-            torch.save(checkpoint_dict, checkpoint_path)
         step += 1
         print('Epoch: ', step)
-    val_loss, average_corr = validate_model()
-    epoch_train_losses.append(np.mean(losses))
-    epoch_val_losses.append(val_loss)
-    epoch_avg_corr.append(average_corr)
-    checkpoint_dict = {
-                "model_state_dict": model.state_dict(),
-                "optimizer_state_dict": optimizer.state_dict(),
-                "loss": loss,
-                "step": step,
-                "epoch": epoch_ind,
-                "epoch_val_losses": epoch_val_losses,
-                "epoch_train_losses": epoch_train_losses,
-                "epoch_avg_corr" : epoch_avg_corr,
-                "best_avg_corr": best_average_corr
-            }
-    if (average_corr > best_average_corr):
-        best_average_corr = average_corr
-        checkpoint_dict["best_avg_corr"] = best_average_corr
-        best_checkpoint_dict = checkpoint_dict
-        torch.save(best_checkpoint_dict, best_checkpoint_path)
-    torch.save(checkpoint_dict, checkpoint_path)
+		val_loss, average_corr = validate_model()
+		epoch_train_losses.append(np.mean(losses))
+		epoch_val_losses.append(val_loss)
+		epoch_avg_corr.append(average_corr)
+		checkpoint_dict = {
+								"model_state_dict": model.state_dict(),
+								"optimizer_state_dict": optimizer.state_dict(),
+								"loss": loss,
+								"step": step,
+								"epoch": epoch_ind,
+								"epoch_val_losses": epoch_val_losses,
+								"epoch_train_losses": epoch_train_losses,
+								"epoch_avg_corr" : epoch_avg_corr,
+								"best_avg_corr": best_average_corr
+						}
+		if (average_corr > best_average_corr):
+				best_average_corr = average_corr
+				checkpoint_dict["best_avg_corr"] = best_average_corr
+				best_checkpoint_dict = checkpoint_dict
+				torch.save(best_checkpoint_dict, best_checkpoint_path)
+		torch.save(checkpoint_dict, checkpoint_path)
```

### Comparing `HACNet-1.0.1/HACNet/functions.py` & `HACNet-1.3.2/HACNet/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         cnn_model.to(device)
         if isinstance(cnn_model, (DistributedDataParallel, DataParallel)):
             cnn_model = cnn_model.module
         # load checkpoint file
         cnn_checkpoint = torch.load(cnn_checkpoint_path, map_location=device)
         # model state dict
         cnn_model_state_dict = cnn_checkpoint.pop("model_state_dict")
-        cnn_model.load_state_dict(cnn_model_state_dict, strict=False)
+        cnn_model.load_state_dict(cnn_model_state_dict, strict=True)
         # create empty arrays to hold predicted and true values
         y_true_cnn = np.zeros((len(cnn_dataset),), dtype=np.float32)
         y_pred_cnn = np.zeros((len(cnn_dataset),), dtype=np.float32)
         pdbid_arr = np.zeros((len(cnn_dataset),), dtype=object)
         pred_list = []
         cnn_model.eval()
         with torch.no_grad():
@@ -96,15 +96,15 @@
         gcn0_dataloader = DataListLoader(gcn0_dataset, batch_size=7, shuffle=False)
         # define model
         gcn0_model = GeometricDataParallel(GCN(in_channels=20, gather_width=128, prop_iter=4, dist_cutoff=3.5)).float()
         # load checkpoint file
         gcn0_checkpoint = torch.load(gcn0_checkpoint_path, map_location=device)
         # model state dict
         gcn0_model_state_dict = gcn0_checkpoint.pop("model_state_dict")
-        gcn0_model.load_state_dict(gcn0_model_state_dict, strict=False)
+        gcn0_model.load_state_dict(gcn0_model_state_dict, strict=True)
         test_data_hdf = h5py.File(gcn0_test_path, 'r')
         gcn0_model.eval()
         y_true_gcn0, y_pred_gcn0, pdbid_array = [], [], []
         with torch.no_grad():
             for batch in tqdm(gcn0_dataloader):
                 data_list = []
                 for dataset in batch:
@@ -134,15 +134,15 @@
         gcn1_dataloader = DataListLoader(gcn1_dataset, batch_size=7, shuffle=False)
         # define model
         gcn1_model = GeometricDataParallel(GCN(in_channels=20, gather_width=128, prop_iter=4, dist_cutoff=3.5)).float()
         # load checkpoint file
         gcn1_checkpoint = torch.load(gcn1_checkpoint_path, map_location=device)
         # model state dict
         gcn1_model_state_dict = gcn1_checkpoint.pop("model_state_dict")
-        gcn1_model.load_state_dict(gcn1_model_state_dict, strict=False)
+        gcn1_model.load_state_dict(gcn1_model_state_dict, strict=True)
         test_data_hdf = h5py.File(gcn1_test_path, 'r')
         gcn1_model.eval()
         y_true_gcn1, y_pred_gcn1, pdbid_array = [], [], []
         with torch.no_grad():
             for batch in tqdm(gcn1_dataloader):
                 data_list = []
                 for dataset in batch:
```

### Comparing `HACNet-1.0.1/LICENSE` & `HACNet-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `HACNet-1.0.1/README.md` & `HACNet-1.3.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ![hacnet_logo-removebg-preview (2)](https://user-images.githubusercontent.com/98780179/198727732-de8a6370-0086-4d1e-a827-e7de432f2716.png)
 
-![image](https://user-images.githubusercontent.com/98780179/211015762-b1d34b03-839a-459f-a0ae-b14450e453b1.png)
-
 # HAC-Net: A Hybrid Attention-Based Convolutional Neural Network for Highly Accurate Protein-Ligand Binding Affinity Prediction
 
+![image](https://user-images.githubusercontent.com/98780179/211151322-15544a37-9dd2-42b2-b843-01138dd01f49.png)
+
 ## Summary
 Applying deep learning concepts from image detection and graph theory has greatly advanced protein-ligand binding affinity prediction, a challenge with enormous ramifications for both drug discovery and protein engineering. We build upon these advances by designing a novel deep learning architecture consisting of a 3-dimensional convolutional neural network utilizing channel-wise attention and two graph convolutional networks utilizing attention-based aggregation of node features. HAC-Net (Hybrid Attention-Based Convolutional Neural Network) obtains state-of-the-art results on the PDBbind v.2016 core set, the most widely recognized benchmark in the field. We extensively assess the generalizability of our model using multiple train-test splits, each of which maximizes differences between either protein structures, protein sequences, or ligand extended-connectivity fingerprints. Furthermore, we perform 10-fold cross-validation with a similarity cutoff between SMILES strings of ligands in the training and test sets, and also evaluate the performance of HAC-Net on lower-quality data. We envision that this model can be extended to a broad range of supervised learning problems related to structure-based biomolecular property prediction.
 
 ## Overview of Model
 
 ![ezgif com-gif-maker (4)](https://user-images.githubusercontent.com/98780179/206188596-032a4f78-4af1-48e8-8cc0-f1800587ddab.gif)
 
@@ -18,14 +18,17 @@
 1) HDF files used for training, validation and testing
 2) NPY files containing 3D-CNN extracted features
 3) PT files containing model parameters
 4) IPYNB files of tutorial notebooks for training and testing
 
 can be found at: https://drive.google.com/drive/folders/1yB2voUxwzhrQRh0JXnOD3BzY8ZQrbgUK?usp=sharing
 
+## Associated Journal Article
+https://pubs.acs.org/doi/10.1021/acs.jcim.3c00251
+
 ## Associated Preprint
 https://arxiv.org/abs/2212.12440
 
 ## Python Package
 https://pypi.org/project/HACNet/
 
 in order to install the HACNet package, simply run:
```

