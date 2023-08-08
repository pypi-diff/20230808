# Comparing `tmp/keypoint-moseq-0.1.5.tar.gz` & `tmp/keypoint-moseq-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keypoint-moseq-0.1.5.tar", last modified: Thu Jun  8 14:24:39 2023, max compression
+gzip compressed data, was "keypoint-moseq-0.2.0.tar", last modified: Tue Aug  8 13:46:54 2023, max compression
```

## Comparing `keypoint-moseq-0.1.5.tar` & `keypoint-moseq-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-06-08 14:24:39.510188 keypoint-moseq-0.1.5/
--rw-r--r--   0 calebweinreb   (501) staff       (20)     8355 2023-04-19 14:03:24.000000 keypoint-moseq-0.1.5/LICENSE.md
--rw-r--r--   0 calebweinreb   (501) staff       (20)      725 2023-04-19 14:03:24.000000 keypoint-moseq-0.1.5/NOTICE.md
--rw-r--r--   0 calebweinreb   (501) staff       (20)      333 2023-06-08 14:24:39.510313 keypoint-moseq-0.1.5/PKG-INFO
--rw-r--r--   0 calebweinreb   (501) staff       (20)     1426 2023-05-16 23:54:35.000000 keypoint-moseq-0.1.5/README.md
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-06-08 14:24:39.511103 keypoint-moseq-0.1.5/keypoint_moseq/
--rw-r--r--   0 calebweinreb   (501) staff       (20)     1007 2023-06-06 15:33:16.000000 keypoint-moseq-0.1.5/keypoint_moseq/__init__.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)      497 2023-06-08 14:24:39.511192 keypoint-moseq-0.1.5/keypoint_moseq/_version.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    28353 2023-06-06 15:33:16.000000 keypoint-moseq-0.1.5/keypoint_moseq/analysis.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    17701 2023-06-06 15:33:16.000000 keypoint-moseq-0.1.5/keypoint_moseq/calibration.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    17249 2023-06-06 15:33:16.000000 keypoint-moseq-0.1.5/keypoint_moseq/fitting.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    46577 2023-06-08 14:18:49.000000 keypoint-moseq-0.1.5/keypoint_moseq/io.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    27260 2023-06-06 15:33:16.000000 keypoint-moseq-0.1.5/keypoint_moseq/util.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    68266 2023-06-08 13:46:30.000000 keypoint-moseq-0.1.5/keypoint_moseq/viz.py
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-06-08 14:24:39.509860 keypoint-moseq-0.1.5/keypoint_moseq.egg-info/
--rw-r--r--   0 calebweinreb   (501) staff       (20)      333 2023-06-08 14:24:39.000000 keypoint-moseq-0.1.5/keypoint_moseq.egg-info/PKG-INFO
--rw-r--r--   0 calebweinreb   (501) staff       (20)      455 2023-06-08 14:24:39.000000 keypoint-moseq-0.1.5/keypoint_moseq.egg-info/SOURCES.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)        1 2023-06-08 14:24:39.000000 keypoint-moseq-0.1.5/keypoint_moseq.egg-info/dependency_links.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)      170 2023-06-08 14:24:39.000000 keypoint-moseq-0.1.5/keypoint_moseq.egg-info/requires.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)       15 2023-06-08 14:24:39.000000 keypoint-moseq-0.1.5/keypoint_moseq.egg-info/top_level.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)      752 2023-06-08 14:24:39.510854 keypoint-moseq-0.1.5/setup.cfg
--rw-r--r--   0 calebweinreb   (501) staff       (20)      246 2023-06-06 15:33:16.000000 keypoint-moseq-0.1.5/setup.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    83607 2023-05-04 15:16:47.000000 keypoint-moseq-0.1.5/versioneer.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-08-08 13:46:54.084265 keypoint-moseq-0.2.0/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     8355 2023-04-19 14:03:24.000000 keypoint-moseq-0.2.0/LICENSE.md
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      725 2023-04-19 14:03:24.000000 keypoint-moseq-0.2.0/NOTICE.md
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      333 2023-08-08 13:46:54.084452 keypoint-moseq-0.2.0/PKG-INFO
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     1426 2023-05-16 23:54:35.000000 keypoint-moseq-0.2.0/README.md
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-08-08 13:46:54.086022 keypoint-moseq-0.2.0/keypoint_moseq/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      560 2023-08-08 13:43:41.000000 keypoint-moseq-0.2.0/keypoint_moseq/__init__.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      497 2023-08-08 13:46:54.086142 keypoint-moseq-0.2.0/keypoint_moseq/_version.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    57548 2023-08-08 13:43:41.000000 keypoint-moseq-0.2.0/keypoint_moseq/analysis.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    18196 2023-08-08 13:43:41.000000 keypoint-moseq-0.2.0/keypoint_moseq/calibration.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    12577 2023-08-08 13:43:41.000000 keypoint-moseq-0.2.0/keypoint_moseq/fitting.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    41633 2023-08-08 13:43:41.000000 keypoint-moseq-0.2.0/keypoint_moseq/io.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    38374 2023-08-08 13:43:41.000000 keypoint-moseq-0.2.0/keypoint_moseq/util.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    70904 2023-08-08 13:43:41.000000 keypoint-moseq-0.2.0/keypoint_moseq/viz.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    21422 2023-08-08 13:43:41.000000 keypoint-moseq-0.2.0/keypoint_moseq/widgets.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-08-08 13:46:54.083712 keypoint-moseq-0.2.0/keypoint_moseq.egg-info/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      333 2023-08-08 13:46:53.000000 keypoint-moseq-0.2.0/keypoint_moseq.egg-info/PKG-INFO
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      481 2023-08-08 13:46:53.000000 keypoint-moseq-0.2.0/keypoint_moseq.egg-info/SOURCES.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)        1 2023-08-08 13:46:53.000000 keypoint-moseq-0.2.0/keypoint_moseq.egg-info/dependency_links.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      296 2023-08-08 13:46:53.000000 keypoint-moseq-0.2.0/keypoint_moseq.egg-info/requires.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)       15 2023-08-08 13:46:53.000000 keypoint-moseq-0.2.0/keypoint_moseq.egg-info/top_level.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      887 2023-08-08 13:46:54.085603 keypoint-moseq-0.2.0/setup.cfg
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      247 2023-08-08 13:43:41.000000 keypoint-moseq-0.2.0/setup.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    84134 2023-08-08 13:43:41.000000 keypoint-moseq-0.2.0/versioneer.py
```

### Comparing `keypoint-moseq-0.1.5/LICENSE.md` & `keypoint-moseq-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.1.5/NOTICE.md` & `keypoint-moseq-0.2.0/NOTICE.md`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.1.5/README.md` & `keypoint-moseq-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.1.5/keypoint_moseq/calibration.py` & `keypoint-moseq-0.2.0/keypoint_moseq/calibration.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,449 +2,557 @@
 import tqdm
 import os
 from textwrap import fill
 from vidio.read import OpenCVReader
 from keypoint_moseq.io import update_config
 from keypoint_moseq.util import find_matching_videos, get_edges
 
-def sample_error_frames(confidences, bodyparts, use_bodyparts,
-                        num_bins=10, num_samples=100, num_videos=10,
-                        conf_pseudocount=1e-3):
-    """
-    Randomly sample frames, enriching for those with low confidence 
-    keypoint detections.
+
+def sample_error_frames(
+    confidences,
+    bodyparts,
+    use_bodyparts,
+    num_bins=10,
+    num_samples=100,
+    conf_pseudocount=1e-3,
+):
+    """Randomly sample frames, enriching for those with low confidence keypoint
+    detections.
 
     Parameters
     ----------
     confidences: dict
-        Keypoint detection confidences for a collection of sessions 
+        Keypoint detection confidences for a collection of recordings
 
     bodyparts: list
         Label for each keypoint represented in `confidences`
 
     use_bodyparts: list
         Ordered subset of keypoint labels to be used for modeling
 
     num_bins: int, default=10
         Number of bins to use for enriching low-confidence keypoint
-        detections. Confidence values for all used keypoints are 
+        detections. Confidence values for all used keypoints are
         divided into log-spaced bins and an equal number of instances
         are sampled from each bin.
 
     num_samples: int, default=100
         Total number of frames to sample
 
-    num_videos: int, default=10
-        Maximum number of videos to use. Fewer videos helps with
-        faster frame loading.
-
     conf_pseudocount: float, default=1e-3
         Pseudocount used to augment keypoint confidences.
-        
+
     Returns
     -------
     sample_keys: list of tuples
-        List of sampled frames as tuples with format 
+        List of sampled frames as tuples with format
         (key, frame_number, bodypart)
-
     """
-    confidences = {k:v+conf_pseudocount for k,v in confidences.items()}
-    all_videos = sorted(confidences.keys())
-    num_videos = min(num_videos, len(all_videos))
-    use_videos = np.random.choice(all_videos, num_videos, replace=False)
-    
+    confidences = {k: v + conf_pseudocount for k, v in confidences.items()}
     all_confs = np.concatenate([v.flatten() for v in confidences.values()])
     min_conf, max_conf = np.nanmin(all_confs), np.nanmax(all_confs)
     thresholds = np.logspace(np.log10(min_conf), np.log10(max_conf), num_bins)
-    mask = np.array([bp in use_bodyparts for bp in bodyparts])[None,:]
-        
+    mask = np.array([bp in use_bodyparts for bp in bodyparts])[None, :]
+
     sample_keys = []
-    for low,high in zip(thresholds[:-1],thresholds[1:]):
-        
+    for low, high in zip(thresholds[:-1], thresholds[1:]):
         samples_in_bin = []
-        for key,confs in confidences.items():
-            for t,k in zip(*np.nonzero((confs>=low)*(confs<high)*mask)): 
-                samples_in_bin.append((key,t,bodyparts[k]))
-        
-        if len(samples_in_bin)>0:
-            n = min(num_samples//num_bins, len(samples_in_bin))
-            for i in np.random.choice(len(samples_in_bin), n, replace=False): 
+        for key, confs in confidences.items():
+            for t, k in zip(
+                *np.nonzero((confs >= low) * (confs < high) * mask)
+            ):
+                samples_in_bin.append((key, t, bodyparts[k]))
+
+        if len(samples_in_bin) > 0:
+            n = min(num_samples // num_bins, len(samples_in_bin))
+            for i in np.random.choice(len(samples_in_bin), n, replace=False):
                 sample_keys.append(samples_in_bin[i])
-            
-    sample_keys = [sample_keys[i] for i in np.random.permutation(len(sample_keys))]    
+
+    sample_keys = [
+        sample_keys[i] for i in np.random.permutation(len(sample_keys))
+    ]
     return sample_keys
 
 
 def load_sampled_frames(sample_keys, video_dir, video_extension=None):
-    """
-    Load sampled frames from a directory of videos.
+    """Load sampled frames from a directory of videos.
 
     Parameters
     ----------
     sample_keys: list of tuples
-        List of sampled frames as tuples with format 
+        List of sampled frames as tuples with format
         (key, frame_number, bodypart)
 
     video_dir: str
         Path to directory containing videos
 
     video_extension: str, default=None
         Preferred video extension (passed to :py:func:`keypoint_moseq.util.find_matching_videos`)
 
     Returns
     -------
     sample_keys: dict
         Dictionary mapping elements from `sample_keys` to the
         corresponding videos frames.
-
     """
     keys = sorted(set([k[0] for k in sample_keys]))
-    videos = find_matching_videos(keys,video_dir)
-    key_to_video = dict(zip(keys,videos))
-    readers = {key: OpenCVReader(video) for key,video in zip(keys,videos)}
-    pbar = tqdm.tqdm(sample_keys, desc='Loading sample frames', position=0, leave=True)
-    return {(key,frame,bodypart):readers[key][frame] for key,frame,bodypart in pbar}
+    videos = find_matching_videos(keys, video_dir)
+    key_to_video = dict(zip(keys, videos))
+    readers = {key: OpenCVReader(video) for key, video in zip(keys, videos)}
+    pbar = tqdm.tqdm(
+        sample_keys,
+        desc="Loading sample frames",
+        position=0,
+        leave=True,
+        ncols=72,
+    )
+    return {
+        (key, frame, bodypart): readers[key][frame]
+        for key, frame, bodypart in pbar
+    }
 
 
 def load_annotations(project_dir):
-    """
-    Reload saved calibration annotations.
+    """Reload saved calibration annotations.
 
     Parameters
     ----------
     project_dir: str
         Load annotations from `{project_dir}/error_annotations.csv`
 
     Returns
     -------
     annotations: dict
-        Dictionary mapping sample keys to annotated keypoint 
-        coordinates. (See :py:func:`keypoint_moseq.calibration.sample_error_frames` 
+        Dictionary mapping sample keys to annotated keypoint
+        coordinates. (See :py:func:`keypoint_moseq.calibration.sample_error_frames`
         for format of sample keys)
-    """   
+    """
     annotations = {}
-    annotations_path = os.path.join(
-        project_dir,'error_annotations.csv')
+    annotations_path = os.path.join(project_dir, "error_annotations.csv")
     if os.path.exists(annotations_path):
-        for l in open(annotations_path,'r').read().split('\n')[1:]:
-            key,frame,bodypart,x,y = l.split(',')
-            sample_key = (key,int(frame),bodypart)
-            annotations[sample_key] = (float(x),float(y))
+        for l in open(annotations_path, "r").read().split("\n")[1:]:
+            key, frame, bodypart, x, y = l.split(",")
+            sample_key = (key, int(frame), bodypart)
+            annotations[sample_key] = (float(x), float(y))
     return annotations
-        
-def save_annotations(project_dir, annotations): 
-    """
-    Save calibration annotations to a csv file
+
+
+def save_annotations(project_dir, annotations):
+    """Save calibration annotations to a csv file.
 
     Parameters
     ----------
     project_dir: str
-        Save annotations to `{project_dir}/error_annotations.csv` 
+        Save annotations to `{project_dir}/error_annotations.csv`
 
     annotations: dict
-        Dictionary mapping sample keys to annotated keypoint 
-        coordinates. (See :py:func:`keypoint_moseq.calibration.sample_error_frames` 
+        Dictionary mapping sample keys to annotated keypoint
+        coordinates. (See :py:func:`keypoint_moseq.calibration.sample_error_frames`
         for format of sample keys)
     """
-    output = ['key,frame,bodypart,x,y']
-    for (key,frame,bodypart),(x,y) in annotations.items():
-        output.append(f'{key},{frame},{bodypart},{x},{y}')
-    path = os.path.join(project_dir,'error_annotations.csv')        
-    open(path,'w').write('\n'.join(output))
-    print(fill(f'Annotations saved to {path}'))
-    
+    output = ["key,frame,bodypart,x,y"]
+    for (key, frame, bodypart), (x, y) in annotations.items():
+        output.append(f"{key},{frame},{bodypart},{x},{y}")
+    path = os.path.join(project_dir, "error_annotations.csv")
+    open(path, "w").write("\n".join(output))
+    print(fill(f"Annotations saved to {path}"))
+
+
 def save_params(project_dir, estimator):
-    """
-    Save config parameters learned via calibration
+    """Save config parameters learned via calibration.
 
     Parameters
     ----------
     project_dir: str
-        Save parameters `{project_dir}/config.yml` 
+        Save parameters `{project_dir}/config.yml`
 
     estimator: :py:func:`holoviews.streams.Stream`
         Stream object with fields `conf_threshold`, `slope`, `intercept`
     """
-    update_config(project_dir, 
-                  conf_threshold=float(estimator.conf_threshold),
-                  slope=float(estimator.slope), 
-                  intercept=float(estimator.intercept))
+    update_config(
+        project_dir,
+        conf_threshold=float(estimator.conf_threshold),
+        slope=float(estimator.slope),
+        intercept=float(estimator.intercept),
+    )
 
 
-def _confs_and_dists_from_annotations(coordinates, confidences, 
-                                      annotations, bodyparts):
-    confs,dists = [],[]
-    for (key,frame,bodypart),xy in annotations.items():
+def _confs_and_dists_from_annotations(
+    coordinates, confidences, annotations, bodyparts
+):
+    confs, dists = [], []
+    for (key, frame, bodypart), xy in annotations.items():
         if key in coordinates and key in confidences:
             k = bodyparts.index(bodypart)
             confs.append(confidences[key][frame][k])
-            dists.append(np.sqrt(((coordinates[key][frame][k]-np.array(xy))**2).sum()))
-    return confs,dists
-
-
-def _noise_calibration_widget(project_dir, coordinates, confidences,
-                              sample_keys, sample_images, annotations, *, 
-                              keypoint_colormap, bodyparts, skeleton, 
-                              error_estimator, conf_threshold, **kwargs):
-    
+            dists.append(
+                np.sqrt(
+                    ((coordinates[key][frame][k] - np.array(xy)) ** 2).sum()
+                )
+            )
+    return confs, dists
+
+
+def _noise_calibration_widget(
+    project_dir,
+    coordinates,
+    confidences,
+    sample_keys,
+    sample_images,
+    annotations,
+    *,
+    keypoint_colormap,
+    bodyparts,
+    skeleton,
+    error_estimator,
+    conf_threshold,
+    **kwargs,
+):
     from scipy.stats import linregress
     from holoviews.streams import Tap, Stream
     import holoviews as hv
     import panel as pn
-    hv.extension('bokeh')
 
-    max_height = np.max([sample_images[k].shape[0] for k in sample_keys]) 
-    max_width = np.max([sample_images[k].shape[1] for k in sample_keys]) 
-    max_zoom = int(max(max_width,max_height))
+    hv.extension("bokeh")
+
+    max_height = np.max([sample_images[k].shape[0] for k in sample_keys])
+    max_width = np.max([sample_images[k].shape[1] for k in sample_keys])
+    max_zoom = int(max(max_width, max_height))
 
-    edges = np.array(get_edges(bodyparts,skeleton))
+    edges = np.array(get_edges(bodyparts, skeleton))
     conf_vals = np.hstack([v.flatten() for v in confidences.values()])
-    min_conf,max_conf = np.nanpercentile(conf_vals, .01),np.nanmax(conf_vals)
-    
-    annotations_stream = Stream.define('Annotations', annotations=annotations)()
-    current_sample = Stream.define('Current sample', sample_ix=0)()
-    estimator = Stream.define('Estimator', slope=float(error_estimator['slope']),
-                              intercept=float(error_estimator['intercept']), 
-                              conf_threshold=float(conf_threshold))()
-    
+    min_conf, max_conf = np.nanpercentile(conf_vals, 0.01), np.nanmax(
+        conf_vals
+    )
+
+    annotations_stream = Stream.define(
+        "Annotations", annotations=annotations
+    )()
+    current_sample = Stream.define("Current sample", sample_ix=0)()
+    estimator = Stream.define(
+        "Estimator",
+        slope=float(error_estimator["slope"]),
+        intercept=float(error_estimator["intercept"]),
+        conf_threshold=float(conf_threshold),
+    )()
+
     img_tap = Tap(transient=True)
     vline_tap = Tap(transient=True)
-    crop_size = hv.Dimension('Crop size', range=(0,max_zoom), default=200)
-    
-    def update_scatter(x,y, annotations):
-        
-        confs,dists = _confs_and_dists_from_annotations(
-            coordinates, confidences, annotations, bodyparts)
- 
-        log_dists = np.log10(np.array(dists)+1)
+    crop_size = hv.Dimension("Crop size", range=(0, max_zoom), default=200)
+
+    def update_scatter(x, y, annotations):
+        confs, dists = _confs_and_dists_from_annotations(
+            coordinates, confidences, annotations, bodyparts
+        )
+
+        log_dists = np.log10(np.array(dists) + 1)
         log_confs = np.log10(np.maximum(confs, min_conf))
-        max_dist = np.log10(np.sqrt(max_height**2+max_width**2)+1)
+        max_dist = np.log10(np.sqrt(max_height**2 + max_width**2) + 1)
 
-        xspan = np.log10(max_conf)-np.log10(min_conf)
-        xlim = (np.log10(min_conf)-xspan/10, np.log10(max_conf)+xspan/10)
-        ylim = (-max_dist/50,max_dist)
-        
-        if len(log_dists)>1:
-            m,b = linregress(log_confs,log_dists)[:2]
-            estimator.event(slope=m, intercept=b)
-        else: m,b = estimator.slope, estimator.intercept
+        xspan = np.log10(max_conf) - np.log10(min_conf)
+        xlim = (
+            np.log10(min_conf) - xspan / 10,
+            np.log10(max_conf) + xspan / 10,
+        )
+        ylim = (-max_dist / 50, max_dist)
 
-        if x is None: x = np.log10(conf_threshold)
-        else: estimator.event(conf_threshold=10**x)
-        passing_percent = (conf_vals>10**x).mean()*100
-                    
-        scatter = hv.Scatter(zip(log_confs,log_dists)).opts(
-            color='k', size=6, xlim=xlim, ylim=ylim, axiswise=True, 
-            frame_width=250, default_tools=[])
-        
-        curve = hv.Curve([(xlim[0],xlim[0]*m+b),(xlim[1],xlim[1]*m+b)]).opts(
-            xlim=xlim, ylim=ylim, axiswise=True, default_tools=[])  
-        
-        vline_label = hv.Text(x-(xlim[1]-xlim[0])/50, ylim[1]-(ylim[1]-ylim[0])/100,
-            f'confidence\nthreshold\n{10**x:.5f}\n({passing_percent:.1f}%)').opts(
-            axiswise=True, text_align='right', text_baseline='top', 
-            text_font_size="8pt", default_tools=[])
-        
-        vline = hv.VLine(x).opts(
-            axiswise=True, line_dash='dashed', color='lightgray',  default_tools=[])
+        if len(log_dists) > 1:
+            m, b = linregress(log_confs, log_dists)[:2]
+            estimator.event(slope=m, intercept=b)
+        else:
+            m, b = estimator.slope, estimator.intercept
 
-        return (scatter*curve*vline*vline_label).opts(
-            toolbar=None, default_tools=[], 
-            xlabel='log10(confidence)', ylabel='log10(error)')
+        if x is None:
+            x = np.log10(conf_threshold)
+        else:
+            estimator.event(conf_threshold=10**x)
+        passing_percent = (conf_vals > 10**x).mean() * 100
+
+        scatter = hv.Scatter(zip(log_confs, log_dists)).opts(
+            color="k",
+            size=6,
+            xlim=xlim,
+            ylim=ylim,
+            axiswise=True,
+            frame_width=250,
+            default_tools=[],
+        )
+
+        curve = hv.Curve(
+            [(xlim[0], xlim[0] * m + b), (xlim[1], xlim[1] * m + b)]
+        ).opts(xlim=xlim, ylim=ylim, axiswise=True, default_tools=[])
+
+        vline_label = hv.Text(
+            x - (xlim[1] - xlim[0]) / 50,
+            ylim[1] - (ylim[1] - ylim[0]) / 100,
+            f"confidence\nthreshold\n{10**x:.5f}\n({passing_percent:.1f}%)",
+        ).opts(
+            axiswise=True,
+            text_align="right",
+            text_baseline="top",
+            text_font_size="8pt",
+            default_tools=[],
+        )
 
+        vline = hv.VLine(x).opts(
+            axiswise=True,
+            line_dash="dashed",
+            color="lightgray",
+            default_tools=[],
+        )
+
+        return (scatter * curve * vline * vline_label).opts(
+            toolbar=None,
+            default_tools=[],
+            xlabel="log10(confidence)",
+            ylabel="log10(error)",
+        )
 
     def update_img(crop_size, sample_ix, x, y):
-        
-        key,frame,bodypart = sample_key = sample_keys[sample_ix]
+        key, frame, bodypart = sample_key = sample_keys[sample_ix]
         image = sample_images[sample_key]
-        h,w = image.shape[:2]
+        h, w = image.shape[:2]
 
         keypoint_ix = bodyparts.index(bodypart)
         xys = coordinates[key][frame].copy()
-        xys[:,1] = h-xys[:,1]
+        xys[:, 1] = h - xys[:, 1]
         masked_nodes = np.nonzero(~np.isnan(xys).any(1))[0]
         confs = confidences[key][frame]
-        
+
         if x and y:
-            annotations_stream.annotations.update({sample_key:(x,h-y)})
+            annotations_stream.annotations.update({sample_key: (x, h - y)})
             annotations_stream.event()
 
-        if sample_key in annotations_stream.annotations: 
+        if sample_key in annotations_stream.annotations:
             point = np.array(annotations_stream.annotations[sample_key])
-            point[1] = h-point[1]
-        else: point = xys[keypoint_ix]
-          
-        colorvals = np.linspace(0,1,len(bodyparts))
-        pt_data = np.append(point,colorvals[keypoint_ix])[None]
-        hv_point = hv.Points(pt_data, vdims=['bodypart']).opts(
-            color='bodypart', cmap='autumn', size=15, framewise=True, marker='x', line_width=3)
-        
-        label = f'{bodypart}, confidence = {confs[keypoint_ix]:.5f}'
-        rgb = hv.RGB(image, bounds=(0,0,w,h), label=label).opts(
-            framewise=True, xaxis='bare', yaxis='bare', frame_width=250)
-
-        xlim = (xys[keypoint_ix,0]-crop_size/2,xys[keypoint_ix,0]+crop_size/2)
-        ylim = (xys[keypoint_ix,1]-crop_size/2,xys[keypoint_ix,1]+crop_size/2)
-         
-        edge_data = ((),(),())
-        if len(edges)>0: 
-            masked_edges = edges[np.isin(edges,masked_nodes).all(1)]
-            if len(masked_edges)>0:
-                edge_data = (*masked_edges.T, colorvals[masked_edges[:,0]])
-
-        sizes = np.where(np.arange(len(xys))==keypoint_ix, 10, 6)[masked_nodes]
+            point[1] = h - point[1]
+        else:
+            point = xys[keypoint_ix]
+
+        colorvals = np.linspace(0, 1, len(bodyparts))
+        pt_data = np.append(point, colorvals[keypoint_ix])[None]
+        hv_point = hv.Points(pt_data, vdims=["bodypart"]).opts(
+            color="bodypart",
+            cmap="autumn",
+            size=15,
+            framewise=True,
+            marker="x",
+            line_width=3,
+        )
+
+        label = f"{bodypart}, confidence = {confs[keypoint_ix]:.5f}"
+        rgb = hv.RGB(image, bounds=(0, 0, w, h), label=label).opts(
+            framewise=True, xaxis="bare", yaxis="bare", frame_width=250
+        )
+
+        xlim = (
+            xys[keypoint_ix, 0] - crop_size / 2,
+            xys[keypoint_ix, 0] + crop_size / 2,
+        )
+        ylim = (
+            xys[keypoint_ix, 1] - crop_size / 2,
+            xys[keypoint_ix, 1] + crop_size / 2,
+        )
+
+        edge_data = ((), (), ())
+        if len(edges) > 0:
+            masked_edges = edges[np.isin(edges, masked_nodes).all(1)]
+            if len(masked_edges) > 0:
+                edge_data = (*masked_edges.T, colorvals[masked_edges[:, 0]])
+
+        sizes = np.where(np.arange(len(xys)) == keypoint_ix, 10, 6)[
+            masked_nodes
+        ]
         masked_bodyparts = [bodyparts[i] for i in masked_nodes]
-        nodes = hv.Nodes((*xys[masked_nodes].T, masked_nodes, masked_bodyparts, sizes), vdims=['name','size'])        
-        graph = hv.Graph((edge_data, nodes), vdims='ecolor').opts(
-            node_color='name', node_cmap=keypoint_colormap, tools=[],
-            edge_color='ecolor', edge_cmap=keypoint_colormap, node_size='size')
-
-        return (rgb*graph*hv_point).opts(data_aspect=1, xlim=xlim, ylim=ylim, toolbar=None)
-    
-    
+        nodes = hv.Nodes(
+            (*xys[masked_nodes].T, masked_nodes, masked_bodyparts, sizes),
+            vdims=["name", "size"],
+        )
+        graph = hv.Graph((edge_data, nodes), vdims="ecolor").opts(
+            node_color="name",
+            node_cmap=keypoint_colormap,
+            tools=[],
+            edge_color="ecolor",
+            edge_cmap=keypoint_colormap,
+            node_size="size",
+        )
+
+        return (rgb * graph * hv_point).opts(
+            data_aspect=1, xlim=xlim, ylim=ylim, toolbar=None
+        )
+
     def update_estimator_text(*, slope, intercept, conf_threshold):
-        lines = [f'slope: {slope:.6f}',
-                 f'intercept: {intercept:.6f}',
-                 f'conf_threshold: {conf_threshold:.6f}']
-        estimator_textbox.value='<br>'.join(lines)
-               
-    prev_button = pn.widgets.Button(name='\u25c0', width=50, align='center')
-    next_button = pn.widgets.Button(name='\u25b6', width=50, align='center')
-    save_button = pn.widgets.Button(name='Save:', width=100, align='center')
-    sample_slider = pn.widgets.IntSlider(name='sample', value=0, start=0, end=len(sample_keys), width=100, align='center')
-    zoom_slider = pn.widgets.IntSlider(name='Zoom', value=200, start=1, end=max_zoom, width=100, align='center')
-    estimator_textbox = pn.widgets.StaticText(align='center')
-    
+        lines = [
+            f"slope: {slope:.6f}",
+            f"intercept: {intercept:.6f}",
+            f"conf_threshold: {conf_threshold:.6f}",
+        ]
+        estimator_textbox.value = "<br>".join(lines)
+
+    prev_button = pn.widgets.Button(name="\u25c0", width=50, align="center")
+    next_button = pn.widgets.Button(name="\u25b6", width=50, align="center")
+    save_button = pn.widgets.Button(name="Save:", width=100, align="center")
+    sample_slider = pn.widgets.IntSlider(
+        name="sample",
+        value=0,
+        start=0,
+        end=len(sample_keys),
+        width=100,
+        align="center",
+    )
+    zoom_slider = pn.widgets.IntSlider(
+        name="Zoom",
+        value=200,
+        start=1,
+        end=max_zoom,
+        width=100,
+        align="center",
+    )
+    estimator_textbox = pn.widgets.StaticText(align="center")
+
     def next_sample(event):
-        if current_sample.sample_ix < len(sample_keys)-1:
-            current_sample.event(sample_ix=int(current_sample.sample_ix)+1)
-        sample_slider.value=int(current_sample.sample_ix)
-        
+        if current_sample.sample_ix < len(sample_keys) - 1:
+            current_sample.event(sample_ix=int(current_sample.sample_ix) + 1)
+        sample_slider.value = int(current_sample.sample_ix)
+
     def prev_sample(event):
         if current_sample.sample_ix > 0:
-            current_sample.event(sample_ix=int(current_sample.sample_ix)-1)
-        sample_slider.value=int(current_sample.sample_ix) 
-        
+            current_sample.event(sample_ix=int(current_sample.sample_ix) - 1)
+        sample_slider.value = int(current_sample.sample_ix)
+
     def save_all(event):
         save_annotations(project_dir, annotations_stream.annotations)
         save_params(project_dir, estimator)
-    
+
     @pn.depends(sample_slider.param.value, watch=True)
     def change_sample(value):
         current_sample.event(sample_ix=int(value))
-    
+
     prev_button.on_click(prev_sample)
     next_button.on_click(next_sample)
     save_button.on_click(save_all)
     estimator.add_subscriber(update_estimator_text)
     estimator.event()
 
     img_dmap = hv.DynamicMap(
         pn.bind(update_img, crop_size=zoom_slider),
-        streams=[current_sample, img_tap]
+        streams=[current_sample, img_tap],
     ).opts(framewise=True)
-    
+
     scatter_dmap = hv.DynamicMap(
-        update_scatter, streams=[annotations_stream, vline_tap],
+        update_scatter,
+        streams=[annotations_stream, vline_tap],
     ).opts(framewise=True, axiswise=True)
 
     controls = pn.Row(
-        prev_button, next_button,
+        prev_button,
+        next_button,
         # sample_slider,
-        pn.Spacer(sizing_mode='stretch_width'),
-        zoom_slider, 
-        pn.Spacer(sizing_mode='stretch_width'),
-        save_button,   
-        pn.Spacer(sizing_mode='stretch_width'),
-        estimator_textbox
-    )
-    plots = pn.Row(
-        img_dmap, 
-        scatter_dmap
+        pn.Spacer(sizing_mode="stretch_width"),
+        zoom_slider,
+        pn.Spacer(sizing_mode="stretch_width"),
+        save_button,
+        pn.Spacer(sizing_mode="stretch_width"),
+        estimator_textbox,
     )
+    plots = pn.Row(img_dmap, scatter_dmap)
     return pn.Column(controls, plots)
 
 
-
-
-def noise_calibration(project_dir, coordinates, confidences, *, 
-                      bodyparts, use_bodyparts, video_dir, 
-                      video_extension=None, conf_pseudocount=0.001, 
-                      verbose=False, **kwargs):
-    """
-    Perform manual annotation to calibrate the relationship between
-    keypoint error and neural network confidence. 
-
-    This function creates a widget for interactive annotation in a 
-    jupyter notebook. Users mark correct keypoint locations for a 
-    sequence of frames, and a regression line is fit to the 
+def noise_calibration(
+    project_dir,
+    coordinates,
+    confidences,
+    *,
+    bodyparts,
+    use_bodyparts,
+    video_dir,
+    video_extension=None,
+    conf_pseudocount=0.001,
+    verbose=False,
+    **kwargs,
+):
+    """Perform manual annotation to calibrate the relationship between keypoint
+    error and neural network confidence.
+
+    This function creates a widget for interactive annotation in a
+    jupyter notebook. Users mark correct keypoint locations for a
+    sequence of frames, and a regression line is fit to the
     `log(confidence), log(error)` pairs obtained through annotation.
-    The regression coefficients are used during modeling to set a 
-    prior on the noise level for each keypoint on each frame. 
+    The regression coefficients are used during modeling to set a
+    prior on the noise level for each keypoint on each frame.
 
     Follow these steps to use the widget:
-        - After executing this function, a widget should appear with a 
+        - After executing this function, a widget should appear with a
           video frame in the center.
-        - Annotate the labeled bodypart in each frame by left-clicking 
+        - Annotate the labeled bodypart in each frame by left-clicking
           at the correct location. An "X" should appear there.
-        - Use the arrow buttons and/or sample slider on the left to 
+        - Use the arrow buttons and/or sample slider on the left to
           annotate additional frames.
-        - Each annotation adds a point to the right-hand scatter plot. 
+        - Each annotation adds a point to the right-hand scatter plot.
           Continue until the regression line stabilizes.
-        - At any point, adjust the confidence threshold by clicking on 
-          the scatter plot. The confidence threshold is used to define 
+        - At any point, adjust the confidence threshold by clicking on
+          the scatter plot. The confidence threshold is used to define
           outlier keypoints for PCA and model initialization.
-        - Use the "save" button to store your annotations to disk and 
+        - Use the "save" button to store your annotations to disk and
           save `slope`, `intercept`, and `confidence_threshold`
           to the config.
 
 
     Parameters
     ----------
     project_dir: str
         Project directory. Must contain a `config.yml` file.
 
     coordinates: dict
-        Keypoint coordinates for a collection of sessions. Values
-        must be numpy arrays of shape (T,K,D) where K is the number
-        of keypoints and D={2 or 3}. Keys can be any unique str,
-        but must start with the name of a videofile in `video_dir`. 
+        Keypoint coordinates for a collection of recordings. Values
+        must be numpy arrays of shape (T,K,2) where K is the number
+        of keypoints. Keys can be any unique str, but must start with
+        the name of a videofile in `video_dir`.
 
     confidences: dict
-        Nonnegative confidence values for the keypoints in 
+        Nonnegative confidence values for the keypoints in
         `coordinates` as numpy arrays of shape (T,K).
 
     bodyparts: list
         Label for each keypoint represented in `coordinates`
 
     use_bodyparts: list
         Ordered subset of keypoint labels to be used for modeling
 
     video_dir: str
         Path to directory containing videos. Each video should
         correspond to a key in `coordinates`. The key must
-        contain the videoname as a prefix. 
+        contain the videoname as a prefix.
 
     video_extension: str, default=None
         Preferred video extension (used in :py:func:`keypoint_moseq.util.find_matching_videos`)
 
     conf_pseudocount: float, default=0.001
         Pseudocount added to confidence values to avoid log(0) errors.
 
     verbose: bool, default=False
         Print progress.
     """
-    confidences = {k:v+conf_pseudocount for k,v in confidences.items()}
-    
-    sample_keys = sample_error_frames(
-        confidences, bodyparts, use_bodyparts)
+    dim = list(coordinates.values())[0].shape[-1]
+    assert dim == 2, "Calibration is only supported for 2D keypoints."
+
+    confidences = {k: v + conf_pseudocount for k, v in confidences.items()}
+    sample_keys = sample_error_frames(confidences, bodyparts, use_bodyparts)
 
     annotations = load_annotations(project_dir)
     sample_keys.extend(annotations.keys())
 
     sample_images = load_sampled_frames(
-        sample_keys, video_dir, video_extension=video_extension)
+        sample_keys, video_dir, video_extension=video_extension
+    )
 
     return _noise_calibration_widget(
-        project_dir, coordinates, confidences, sample_keys, 
-        sample_images, annotations, bodyparts=bodyparts, **kwargs)
-
+        project_dir,
+        coordinates,
+        confidences,
+        sample_keys,
+        sample_images,
+        annotations,
+        bodyparts=bodyparts,
+        **kwargs,
+    )
```

### Comparing `keypoint-moseq-0.1.5/keypoint_moseq/io.py` & `keypoint-moseq-0.2.0/keypoint_moseq/io.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,244 +1,290 @@
-from jax.tree_util import tree_map
 import jax.numpy as jnp
 import jax
 import numpy as np
 import warnings
 import h5py
 import joblib
 import tqdm
 import yaml
 import os
-import re
 import pandas as pd
-from datetime import datetime
 from textwrap import fill
-import matplotlib.pyplot as plt
-import tabulate
+import sleap_io
+from pynwb import NWBHDF5IO
+from ndx_pose import PoseEstimation
 
-
-from jax_moseq.utils import batch
-from keypoint_moseq.util import (
-    reindex_by_bodyparts, 
-    list_files_with_exts, 
-    interpolate_keypoints,
-)
+from keypoint_moseq.util import list_files_with_exts, check_nan_proportions
+from jax_moseq.utils import get_frequencies, unbatch
 
 
 def _build_yaml(sections, comments):
     text_blocks = []
-    for title,data in sections:
-        centered_title = f' {title} '.center(50, '=')
+    for title, data in sections:
+        centered_title = f" {title} ".center(50, "=")
         text_blocks.append(f"\n\n{'#'}{centered_title}{'#'}")
-        for key,value in data.items():
-            text = yaml.dump({key:value}).strip('\n')
-            if key in comments: text = f"\n{'#'} {comments[key]}\n{text}"
+        for key, value in data.items():
+            text = yaml.dump({key: value}).strip("\n")
+            if key in comments:
+                text = f"\n{'#'} {comments[key]}\n{text}"
             text_blocks.append(text)
-    return '\n'.join(text_blocks)
-        
+    return "\n".join(text_blocks)
+
+
+def _get_path(
+    project_dir, model_name, path, filename, pathname_for_error_msg="path"
+):
+    if path is None:
+        assert project_dir is not None and model_name is not None, fill(
+            f"`model_name` and `project_dir` are required if `{pathname_for_error_msg}` is None."
+        )
+        path = os.path.join(project_dir, model_name, filename)
+    return path
+
 
 def generate_config(project_dir, **kwargs):
-    """
-    Generate a `config.yml` file with project settings. Default 
-    settings will be used unless overriden by a keyword argument.
-    
+    """Generate a `config.yml` file with project settings. Default settings
+    will be used unless overriden by a keyword argument.
+
     Parameters
     ----------
-    project_dir: str 
+    project_dir: str
         A file `config.yml` will be generated in this directory.
-    
+
     kwargs
-        Custom project settings.  
+        Custom project settings.
     """
-    
+
     def _update_dict(new, original):
-        return {k:new[k] if k in new else v for k,v in original.items()} 
-    
-    hypperams = _update_dict(kwargs, {
-        'error_estimator': {'slope':-.5, 'intercept':.25},
-        'obs_hypparams': {'sigmasq_0':0.1, 'sigmasq_C':.1, 'nu_sigma':1e5, 'nu_s':5},
-        'ar_hypparams': {'latent_dim': 10, 'nlags': 3, 'S_0_scale': 0.01, 'K_0_scale': 10.0},
-        'trans_hypparams': {'num_states': 100, 'gamma': 1e3, 'alpha': 5.7, 'kappa': 1e6},
-        'cen_hypparams': {'sigmasq_loc': 0.5}})
-    
-    hypperams = {k : _update_dict(kwargs, v) for k,v in hypperams.items()}
-
-    anatomy = _update_dict(kwargs, {
-        'bodyparts': ['BODYPART1','BODYPART2','BODYPART3'],
-        'use_bodyparts': ['BODYPART1','BODYPART2','BODYPART3'],
-        'skeleton': [['BODYPART1','BODYPART2'], ['BODYPART2','BODYPART3']],
-        'anterior_bodyparts': ['BODYPART1'],
-        'posterior_bodyparts': ['BODYPART3']})
-        
-    other = _update_dict(kwargs, {
-        'session_name_suffix': '',
-        'verbose':False,
-        'conf_pseudocount': 1e-3,
-        'video_dir': '',
-        'keypoint_colormap': 'autumn',
-        'whiten': True,
-        'fix_heading': False,
-        'seg_length': 10000 })
-       
-    fitting = _update_dict(kwargs, {
-        'added_noise_level': 0.1,
-        'PCA_fitting_num_frames': 1000000,
-        'conf_threshold': 0.5,
-#         'kappa_scan_target_duration': 12,
-#         'kappa_scan_min': 1e2,
-#         'kappa_scan_max': 1e12,
-#         'num_arhmm_scan_iters': 50,
-#         'num_arhmm_final_iters': 200,
-#         'num_kpslds_scan_iters': 50,
-#         'num_kpslds_final_iters': 500
-    })
-    
+        return {k: new[k] if k in new else v for k, v in original.items()}
+
+    hypperams = _update_dict(
+        kwargs,
+        {
+            "error_estimator": {"slope": -0.5, "intercept": 0.25},
+            "obs_hypparams": {
+                "sigmasq_0": 0.1,
+                "sigmasq_C": 0.1,
+                "nu_sigma": 1e5,
+                "nu_s": 5,
+            },
+            "ar_hypparams": {
+                "latent_dim": 10,
+                "nlags": 3,
+                "S_0_scale": 0.01,
+                "K_0_scale": 10.0,
+            },
+            "trans_hypparams": {
+                "num_states": 100,
+                "gamma": 1e3,
+                "alpha": 5.7,
+                "kappa": 1e6,
+            },
+            "cen_hypparams": {"sigmasq_loc": 0.5},
+        },
+    )
+
+    hypperams = {k: _update_dict(kwargs, v) for k, v in hypperams.items()}
+
+    anatomy = _update_dict(
+        kwargs,
+        {
+            "bodyparts": ["BODYPART1", "BODYPART2", "BODYPART3"],
+            "use_bodyparts": ["BODYPART1", "BODYPART2", "BODYPART3"],
+            "skeleton": [
+                ["BODYPART1", "BODYPART2"],
+                ["BODYPART2", "BODYPART3"],
+            ],
+            "anterior_bodyparts": ["BODYPART1"],
+            "posterior_bodyparts": ["BODYPART3"],
+        },
+    )
+
+    other = _update_dict(
+        kwargs,
+        {
+            "recording_name_suffix": "",
+            "verbose": False,
+            "conf_pseudocount": 1e-3,
+            "video_dir": "",
+            "keypoint_colormap": "autumn",
+            "whiten": True,
+            "fix_heading": False,
+            "seg_length": 10000,
+        },
+    )
+
+    fitting = _update_dict(
+        kwargs,
+        {
+            "added_noise_level": 0.1,
+            "PCA_fitting_num_frames": 1000000,
+            "conf_threshold": 0.5,
+            #         'kappa_scan_target_duration': 12,
+            #         'kappa_scan_min': 1e2,
+            #         'kappa_scan_max': 1e12,
+            #         'num_arhmm_scan_iters': 50,
+            #         'num_arhmm_final_iters': 200,
+            #         'num_kpslds_scan_iters': 50,
+            #         'num_kpslds_final_iters': 500
+        },
+    )
+
     comments = {
-        'verbose': 'whether to print progress messages during fitting',
-        'keypoint_colormap': 'colormap used for visualization; see `matplotlib.cm.get_cmap` for options',
-        'added_noise_level': 'upper bound of uniform noise added to the data during initial AR-HMM fitting; this is used to regularize the model',
-        'PCA_fitting_num_frames': 'number of frames used to fit the PCA model during initialization',
-        'video_dir': 'directory with videos from which keypoints were derived (used for crowd movies)',
-        'session_name_suffix': 'suffix used to match videos to session names; this can usually be left empty (see `util.find_matching_videos` for details)',
-        'bodyparts': 'used to access columns in the keypoint data',
-        'skeleton': 'used for visualization only',
-        'use_bodyparts': 'determines the subset of bodyparts to use for modeling and the order in which they are represented',
-        'anterior_bodyparts': 'used to initialize heading',
-        'posterior_bodyparts': 'used to initialize heading',
-        'seg_length': 'data are broken up into segments to parallelize fitting',
-        'trans_hypparams': 'transition hyperparameters',
-        'ar_hypparams': 'autoregressive hyperparameters',
-        'obs_hypparams': 'keypoint observation hyperparameters',
-        'cen_hypparams': 'centroid movement hyperparameters',
-        'error_estimator': 'parameters to convert neural net likelihoods to error size priors',
-        'save_every_n_iters': 'frequency for saving model snapshots during fitting; if 0 only final state is saved', 
-        'kappa_scan_target_duration': 'target median syllable duration (in frames) for choosing kappa',
-        'whiten': 'whether to whiten principal components; used to initialize the latent pose trajectory `x`',
-        'conf_threshold': 'used to define outliers for interpolation when the model is initialized',
-        'conf_pseudocount': 'pseudocount used regularize neural network confidences',
-        'fix_heading': 'whether to keep the heading angle fixed; this should only be True if the pose is constrained to a narrow range of angles, e.g. a headfixed mouse.',
+        "verbose": "whether to print progress messages during fitting",
+        "keypoint_colormap": "colormap used for visualization; see `matplotlib.cm.get_cmap` for options",
+        "added_noise_level": "upper bound of uniform noise added to the data during initial AR-HMM fitting; this is used to regularize the model",
+        "PCA_fitting_num_frames": "number of frames used to fit the PCA model during initialization",
+        "video_dir": "directory with videos from which keypoints were derived (used for crowd movies)",
+        "recording_name_suffix": "suffix used to match videos to recording names; this can usually be left empty (see `util.find_matching_videos` for details)",
+        "bodyparts": "used to access columns in the keypoint data",
+        "skeleton": "used for visualization only",
+        "use_bodyparts": "determines the subset of bodyparts to use for modeling and the order in which they are represented",
+        "anterior_bodyparts": "used to initialize heading",
+        "posterior_bodyparts": "used to initialize heading",
+        "seg_length": "data are broken up into segments to parallelize fitting",
+        "trans_hypparams": "transition hyperparameters",
+        "ar_hypparams": "autoregressive hyperparameters",
+        "obs_hypparams": "keypoint observation hyperparameters",
+        "cen_hypparams": "centroid movement hyperparameters",
+        "error_estimator": "parameters to convert neural net likelihoods to error size priors",
+        "save_every_n_iters": "frequency for saving model snapshots during fitting; if 0 only final state is saved",
+        "kappa_scan_target_duration": "target median syllable duration (in frames) for choosing kappa",
+        "whiten": "whether to whiten principal components; used to initialize the latent pose trajectory `x`",
+        "conf_threshold": "used to define outliers for interpolation when the model is initialized",
+        "conf_pseudocount": "pseudocount used regularize neural network confidences",
+        "fix_heading": "whether to keep the heading angle fixed; this should only be True if the pose is constrained to a narrow range of angles, e.g. a headfixed mouse.",
     }
 
     sections = [
-        ('ANATOMY', anatomy),
-        ('FITTING', fitting),
-        ('HYPER PARAMS',hypperams),
-        ('OTHER', other)
+        ("ANATOMY", anatomy),
+        ("FITTING", fitting),
+        ("HYPER PARAMS", hypperams),
+        ("OTHER", other),
     ]
 
-    with open(os.path.join(project_dir,'config.yml'),'w') as f: 
+    with open(os.path.join(project_dir, "config.yml"), "w") as f:
         f.write(_build_yaml(sections, comments))
-                          
-        
+
+
 def check_config_validity(config):
-    """
-    Check if the config is valid.
+    """Check if the config is valid.
 
     To be valid, the config must satisfy the following criteria:
-        - All the elements of `config["use_bodyparts"]` are 
-          also in `config["bodyparts"]` 
-        - All the elements of `config["anterior_bodyparts"]` are
-          also in `config["bodyparts"]` 
-        - All the elements of `config["anterior_bodyparts"]` are
-          also in `config["bodyparts"]` 
-        - For each pair in `config["skeleton"]`, both elements 
-          also in `config["bodyparts"]` 
+        - All the elements of `config["use_bodyparts"]` are also in
+          `config["bodyparts"]`
+        - All the elements of `config["anterior_bodyparts"]` are also in
+          `config["bodyparts"]`
+        - All the elements of `config["anterior_bodyparts"]` are also in
+          `config["bodyparts"]`
+        - For each pair in `config["skeleton"]`, both elements also in
+          `config["bodyparts"]`
 
     Parameters
     ----------
-    config: dict 
+    config: dict
 
     Returns
     -------
     validity: bool
     """
     error_messages = []
-    
+
     # check anatomy
-    for bodypart in config['use_bodyparts']:
-        if not bodypart in config['bodyparts']:
-            error_messages.append(           
-                f'ACTION REQUIRED: `use_bodyparts` contains {bodypart} '
-                'which is not one of the options in `bodyparts`.')
-            
-    for bodypart in sum(config['skeleton'],[]):
-        if not bodypart in config['bodyparts']:
+    for bodypart in config["use_bodyparts"]:
+        if not bodypart in config["bodyparts"]:
             error_messages.append(
-                f'ACTION REQUIRED: `skeleton` contains {bodypart} '
-                'which is not one of the options in `bodyparts`.')
-            
-    for bodypart in config['anterior_bodyparts']:
-        if not bodypart in config['bodyparts']:
+                f"ACTION REQUIRED: `use_bodyparts` contains {bodypart} "
+                "which is not one of the options in `bodyparts`."
+            )
+
+    for bodypart in sum(config["skeleton"], []):
+        if not bodypart in config["bodyparts"]:
             error_messages.append(
-                f'ACTION REQUIRED: `anterior_bodyparts` contains {bodypart} '
-                'which is not one of the options in `bodyparts`.')
-            
-    for bodypart in config['posterior_bodyparts']:
-        if not bodypart in config['bodyparts']:
-            error_messages.append(     
-                f'ACTION REQUIRED: `posterior_bodyparts` contains {bodypart} '
-                'which is not one of the options in `bodyparts`.')
+                f"ACTION REQUIRED: `skeleton` contains {bodypart} "
+                "which is not one of the options in `bodyparts`."
+            )
 
-    if len(error_messages)==0: 
+    for bodypart in config["anterior_bodyparts"]:
+        if not bodypart in config["bodyparts"]:
+            error_messages.append(
+                f"ACTION REQUIRED: `anterior_bodyparts` contains {bodypart} "
+                "which is not one of the options in `bodyparts`."
+            )
+
+    for bodypart in config["posterior_bodyparts"]:
+        if not bodypart in config["bodyparts"]:
+            error_messages.append(
+                f"ACTION REQUIRED: `posterior_bodyparts` contains {bodypart} "
+                "which is not one of the options in `bodyparts`."
+            )
+
+    if len(error_messages) == 0:
         return True
-    for msg in error_messages: 
-        print(fill(msg, width=70, subsequent_indent='  '), end='\n\n')
+    for msg in error_messages:
+        print(fill(msg, width=70, subsequent_indent="  "), end="\n\n")
     return False
-            
+
 
 def load_config(project_dir, check_if_valid=True, build_indexes=True):
-    """
-    Load a project config file.
-    
+    """Load a project config file.
+
     Parameters
     ----------
     project_dir: str
         Directory containing the config file
-        
+
     check_if_valid: bool, default=True
-        Check if the config is valid using 
+        Check if the config is valid using
         :py:func:`keypoint_moseq.io.check_config_validity`
-        
+
     build_indexes: bool, default=True
-        Add keys `"anterior_idxs"` and `"posterior_idxs"` to the 
-        config. Each maps to a jax array indexing the elements of 
-        `config["anterior_bodyparts"]` and 
-        `config["posterior_bodyparts"]` by their order in 
-        `config["use_bodyparts"]`
+        Add keys `"anterior_idxs"` and `"posterior_idxs"` to the config. Each
+        maps to a jax array indexing the elements of
+        `config["anterior_bodyparts"]` and `config["posterior_bodyparts"]` by
+        their order in `config["use_bodyparts"]`
 
     Returns
     -------
     config: dict
     """
-    config_path = os.path.join(project_dir,'config.yml')
-    
-    with open(config_path, 'r') as stream:  
+    config_path = os.path.join(project_dir, "config.yml")
+
+    with open(config_path, "r") as stream:
         config = yaml.safe_load(stream)
 
-    if check_if_valid: 
+    if check_if_valid:
         check_config_validity(config)
-        
+
     if build_indexes:
-        config['anterior_idxs'] = jnp.array(
-            [config['use_bodyparts'].index(bp) for bp in config['anterior_bodyparts']])
-        config['posterior_idxs'] = jnp.array(
-            [config['use_bodyparts'].index(bp) for bp in config['posterior_bodyparts']])
-    
-    if not 'skeleton' in config or config['skeleton'] is None:
-        config['skeleton'] = []
-        
+        config["anterior_idxs"] = jnp.array(
+            [
+                config["use_bodyparts"].index(bp)
+                for bp in config["anterior_bodyparts"]
+            ]
+        )
+        config["posterior_idxs"] = jnp.array(
+            [
+                config["use_bodyparts"].index(bp)
+                for bp in config["posterior_bodyparts"]
+            ]
+        )
+
+    if not "skeleton" in config or config["skeleton"] is None:
+        config["skeleton"] = []
+
     return config
 
+
 def update_config(project_dir, **kwargs):
-    """
-    Update the config file stored at `project_dir/config.yml`.
-     
-    Use keyword arguments to update key/value pairs in the config.
-    To update model hyperparameters, just use the name of the 
-    hyperparameter as the keyword argument. 
+    """Update the config file stored at `project_dir/config.yml`.
+
+    Use keyword arguments to update key/value pairs in the config. To update
+    model hyperparameters, just use the name of the hyperparameter as the
+    keyword argument.
 
     Examples
     --------
     To update `video_dir` to `/path/to/videos`::
 
       >>> update_config(project_dir, video_dir='/path/to/videos')
       >>> print(load_config(project_dir)['video_dir'])
@@ -246,979 +292,895 @@
 
     To update `trans_hypparams['kappa']` to `100`::
 
       >>> update_config(project_dir, kappa=100)
       >>> print(load_config(project_dir)['trans_hypparams']['kappa'])
       100
     """
-    config = load_config(project_dir, check_if_valid=False, build_indexes=False)
+    config = load_config(
+        project_dir, check_if_valid=False, build_indexes=False
+    )
     config.update(kwargs)
     generate_config(project_dir, **config)
-    
-        
-def setup_project(project_dir, deeplabcut_config=None, sleap_file=None,
-                  overwrite=False, **options):
+
+
+def setup_project(
+    project_dir,
+    deeplabcut_config=None,
+    sleap_file=None,
+    nwb_file=None,
+    overwrite=False,
+    **options,
+):
     """
     Setup a project directory with the following structure::
 
         project_dir
         └── config.yml
-    
+
     Parameters
     ----------
-    project_dir: str 
+    project_dir: str
         Path to the project directory (relative or absolute)
-        
+
     deeplabcut_config: str, default=None
-        Path to a deeplabcut config file. Relevant settings, including
-        `'bodyparts'`, `'skeleton'`, `'use_bodyparts'`, and 
-        `'video_dir'` will be imported from the deeplabcut config and 
-        used to initialize the keypoint MoSeq config. (overrided by kwargs). 
+        Path to a deeplabcut config file. Will be used to initialize
+        `bodyparts`, `skeleton`, `use_bodyparts` and `video_dir` in the
+        keypoint MoSeq config. (overrided by kwargs).
 
     sleap_file: str, default=None
-        Path to a sleap hdf5 file for one of the recordings to be modeled. 
-        Relevant settings, including `'bodyparts'`, `'skeleton'`, 
-        and `'use_bodyparts'` will be imported from the sleap file and used 
-        to initialize the keypoint MoSeq config. (overrided by kwargs). 
-        
+        Path to a .hdf5 or .slp file containing predictions for one video. Will
+        be used to initialize `bodyparts`, `skeleton`, and `use_bodyparts` in
+        the keypoint MoSeq config. (overrided by kwargs).
+
+    nwb_file: str, default=None
+        Path to a .nwb file containing predictions for one video. Will be used
+        to initialize `bodyparts`, `skeleton`, and `use_bodyparts` in the
+        keypoint MoSeq config. (overrided by kwargs).
+
     overwrite: bool, default=False
         Overwrite any config.yml that already exists at the path
-        `{project_dir}/config.yml`
-        
+        `{project_dir}/config.yml`.
+
     options
-        Used to initialize config file. Overrides default settings
+        Used to initialize config file. Overrides default settings.
     """
 
     if os.path.exists(project_dir) and not overwrite:
-        print(fill(
-            f'The directory `{project_dir}` already exists. Use '
-            '`overwrite=True` or pick a different name'))
+        print(
+            fill(
+                f"The directory `{project_dir}` already exists. Use "
+                "`overwrite=True` or pick a different name"
+            )
+        )
         return
-        
-    if deeplabcut_config is not None: 
+
+    if deeplabcut_config is not None:
         dlc_options = {}
-        with open(deeplabcut_config, 'r') as stream:           
+        with open(deeplabcut_config, "r") as stream:
             dlc_config = yaml.safe_load(stream)
-            
             if dlc_config is None:
                 raise RuntimeError(
-                    f'{deeplabcut_config} does not exists or is not a'
-                    ' valid yaml file')
-                
-            if 'multianimalproject' in dlc_config and dlc_config['multianimalproject']:
-                dlc_options['bodyparts'] = dlc_config['multianimalbodyparts']
-                dlc_options['use_bodyparts'] = dlc_config['multianimalbodyparts']
+                    f"{deeplabcut_config} does not exists or is not a"
+                    " valid yaml file"
+                )
+            if (
+                "multianimalproject" in dlc_config
+                and dlc_config["multianimalproject"]
+            ):
+                dlc_options["bodyparts"] = dlc_config["multianimalbodyparts"]
+                dlc_options["use_bodyparts"] = dlc_config[
+                    "multianimalbodyparts"
+                ]
             else:
-                dlc_options['bodyparts'] = dlc_config['bodyparts']
-                dlc_options['use_bodyparts'] = dlc_config['bodyparts']
-
-            dlc_options['skeleton'] = dlc_config['skeleton']
-            dlc_options['video_dir'] = os.path.join(dlc_config['project_path'],'videos')
-
+                dlc_options["bodyparts"] = dlc_config["bodyparts"]
+                dlc_options["use_bodyparts"] = dlc_config["bodyparts"]
+            dlc_options["skeleton"] = dlc_config["skeleton"]
+            dlc_options["video_dir"] = os.path.join(
+                dlc_config["project_path"], "videos"
+            )
         options = {**dlc_options, **options}
 
     elif sleap_file is not None:
         sleap_options = {}
-        with h5py.File(sleap_file, 'r') as f:
-
-            node_names = [n.decode('utf-8') for n in f['node_names']]
-            edge_names = [[n.decode('utf-8') for n in edge] for edge in f['edge_names']]
-            
-            sleap_options['bodyparts'] = node_names
-            sleap_options['use_bodyparts'] = node_names
-            sleap_options['skeleton'] = edge_names
-            
+        if os.path.splitext(sleap_file)[1] == ".slp":
+            slp_file = sleap_io.load_slp(sleap_file)
+            assert len(slp_file.skeletons) == 1, fill(
+                f"{sleap_file} contains more than one skeleton. "
+                "This is not currently supported. Please "
+                "open a github issue or email calebsw@gmail.com"
+            )
+            skeleton = slp_file.skeletons[0]
+            node_names = skeleton.node_names
+            edge_names = [
+                [e.source.name, e.destination.name] for e in skeleton.edges
+            ]
+        else:
+            with h5py.File(sleap_file, "r") as f:
+                node_names = [n.decode("utf-8") for n in f["node_names"]]
+                edge_names = [
+                    [n.decode("utf-8") for n in edge]
+                    for edge in f["edge_names"]
+                ]
+        sleap_options["bodyparts"] = node_names
+        sleap_options["use_bodyparts"] = node_names
+        sleap_options["skeleton"] = edge_names
         options = {**sleap_options, **options}
-    
+
+    elif nwb_file is not None:
+        nwb_options = {}
+        with NWBHDF5IO(nwb_file, mode="r", load_namespaces=True) as io:
+            pose_obj = _load_nwb_pose_obj(io, nwb_file)
+            bodyparts = list(pose_obj.nodes[:])
+            nwb_options["bodyparts"] = bodyparts
+            nwb_options["use_bodyparts"] = bodyparts
+            if "edges" in pose_obj.fields:
+                edges = pose_obj.edges[:]
+                skeleton = [[bodyparts[i], bodyparts[j]] for i, j in edges]
+                nwb_options["skeleton"] = skeleton
+        options = {**nwb_options, **options}
+
     if not os.path.exists(project_dir):
         os.makedirs(project_dir)
     generate_config(project_dir, **options)
-            
-    
-def format_data(coordinates, confidences=None, keys=None, 
-                seg_length=None, bodyparts=None, use_bodyparts=None,
-                conf_pseudocount=1e-3, added_noise_level=0.1, **kwargs):
-    """
-    Format keypoint coordinates and confidences for inference.
-
-    Data are transformed as follows:
-        1. Coordinates and confidences are each merged into a single 
-           array using :py:func:`keypoint_moseq.util.batch`. 
-        2. The keypoints axis is reindexed according to the order
-           of elements in `use_bodyparts` with respect to their 
-           initial orer in `bodyparts`.
-        3. Uniform noise proportional to `added_noise_level` is
-           added to the keypoint coordinates to prevent degenerate
-           solutions during fitting. 
-        4. Keypoint confidences are augmented by `conf_pseudocount`.
-        5. Wherever NaNs occur in the coordinates, they are replaced
-           by values imputed using linear interpolation, and the
-           corresponding confidences are set to `conf_pseudocount`.
-    
-    Parameters
-    ----------
-    coordinates: dict
-        Keypoint coordinates for a collection of sessions. Values
-        must be numpy arrays of shape (T,K,D) where K is the number
-        of keypoints and D={2 or 3}. 
-        
-    confidences: dict, default=None
-        Nonnegative confidence values for the keypoints in 
-        `coordinates` as numpy arrays of shape (T,K).
-        
-    keys: list of str, default=None
-        (See :py:func:`keypoint_moseq.util.batch`)
-        
-    bodyparts: list, default=None
-        Label for each keypoint represented in `coordinates`. Required
-        to reindex coordinates and confidences according to `use_bodyparts`.
-
-    use_bodyparts: list, default=None
-        Ordered subset of keypoint labels to be used for modeling.
-        If `use_bodyparts=None`, then all keypoints are used.
-
-    conf_pseudocount: float, default=1e-3
-        Pseudocount used to augment keypoint confidences.
-    
-    seg_length: int, default=None
-        Length of each segment. If `seg_length=None`, a length is 
-        chosen so that no time-series are broken into multiple segments.
-        If all time-series are shorter than `seg_length`, then
-        `seg_length` is set to the length of the shortest time-series.
-        
-    Returns
-    -------
-    data: dict with the following items
-    
-        Y: jax array with shape (n_segs, seg_length, K, D)
-            Keypoint coordinates from all sessions broken into 
-            fixed-length segments.
-            
-        conf: jax array with shape (n_segs, seg_length, K)
-            Confidences from all sessions broken into fixed-length 
-            segments. If no input is provided for `confidences`, 
-            then `data["conf"]=None`.
-        
-        mask: jax array with shape (n_segs, seg_length)
-            Binary array where 0 indicates areas of padding 
-            (see :py:func:`keypoint_moseq.util.batch`).
-            
-    labels: list of tuples (object, int, int)
-        Label for each row of `Y` and `conf` 
-        (see :py:func:`keypoint_moseq.util.batch`).
-    """    
-    if keys is None: 
-        keys = sorted(coordinates.keys()) 
-    else: 
-        bad_keys = set(keys) - set(coordinates.keys())
-        assert len(bad_keys) == 0, fill(
-            f'Keys {bad_keys} not found in coordinates')
-
-    assert len(keys) > 0, 'No sessions found'
-
-    num_keypoints = [coordinates[key].shape[-2] for key in keys]
-    assert len(set(num_keypoints)) == 1, fill(
-        f'All sessions must have the same number of keypoints, but '
-        f'found {set(num_keypoints)} keypoints across sessions.')
-    
-    if bodyparts is not None:
-        assert len(bodyparts) == num_keypoints[0], fill(
-            f'The number of keypoints in `coordinates` ({num_keypoints[0]}) '
-            f'does not match the number of labels in `bodyparts` '
-            f'({len(bodyparts)})')
-
-    if any(['/' in key for key in keys]): 
-        warnings.warn(fill(
-            'WARNING: Session names should not contain "/", this will cause '
-            'problems with saving/loading hdf5 files.'))
-        
-    if confidences is None:
-        confidences = {key: np.ones_like(coordinates[key][...,0]) for key in keys}
-
-    if bodyparts is not None and use_bodyparts is not None:
-        coordinates = reindex_by_bodyparts(coordinates, bodyparts, use_bodyparts)
-        confidences = reindex_by_bodyparts(confidences, bodyparts, use_bodyparts)
-
-    for key in keys:
-        outliers = np.isnan(coordinates[key]).any(-1)
-        coordinates[key] = interpolate_keypoints(coordinates[key], outliers)
-        confidences[key] = np.where(outliers, 0, np.nan_to_num(confidences[key]))
-    
-    if seg_length is not None:
-        max_session_length = max([coordinates[key].shape[0] for key in keys])
-        seg_length = min(seg_length, max_session_length)
-
-    Y,mask,labels = batch(coordinates, seg_length=seg_length, keys=keys)
-    Y = Y.astype(float)
-
-    conf = batch(confidences, seg_length=seg_length, keys=keys)[0]
-    if np.min(conf) < 0: 
-        conf = np.maximum(conf,0) 
-        warnings.warn(fill(
-            'Negative confidence values are not allowed and will be set to 0.'))
-    conf = conf + conf_pseudocount
-  
-    if added_noise_level>0: 
-        Y += np.random.uniform(-added_noise_level,added_noise_level,Y.shape)
-        
-    return jax.device_put({'mask':mask, 'Y':Y, 'conf':conf}), labels
 
 
 def save_pca(pca, project_dir, pca_path=None):
-    """
-    Save a PCA model to disk.
+    """Save a PCA model to disk.
+
+    The model is saved to `pca_path` or else to `{project_dir}/pca.p`.
 
-    The model is saved to `pca_path` or else to 
-    `{project_dir}/pca.p`.
-    
     Parameters
     ----------
     pca: :py:class:`sklearn.decomposition.PCA`
     project_dir: str
     pca_path: str, default=None
     """
-    if pca_path is None: 
-        pca_path = os.path.join(project_dir,'pca.p')
+    if pca_path is None:
+        pca_path = os.path.join(project_dir, "pca.p")
     joblib.dump(pca, pca_path)
-    
+
+
 def load_pca(project_dir, pca_path=None):
-    """
-    Load a PCA model from disk.
+    """Load a PCA model from disk.
 
-    The model is loaded from `pca_path` or else from 
-    `{project_dir}/pca.p`.
+    The model is loaded from `pca_path` or else from `{project_dir}/pca.p`.
 
     Parameters
     ----------
     project_dir: str
     pca_path: str, default=None
 
     Returns
     -------
     pca: :py:class:`sklearn.decomposition.PCA`
-    """ 
+    """
     if pca_path is None:
-        pca_path = os.path.join(project_dir,'pca.p')
+        pca_path = os.path.join(project_dir, "pca.p")
         assert os.path.exists(pca_path), fill(
-            f'No PCA model found at {pca_path}')
+            f"No PCA model found at {pca_path}"
+        )
     return joblib.load(pca_path)
 
 
-def load_last_checkpoint(project_dir):
-    """
-    Load checkpoint for the most recent model.
+def load_checkpoint(
+    project_dir=None, model_name=None, path=None, iteration=None
+):
+    """Load data and model snapshot from a saved checkpoint.
 
-    This method assumes the following directory structure for saved
-    model checkpoints::
-
-        project_dir
-        ├──YYYY_MM_DD-HH_MM_SS
-        │  └checkpoint.p
-        ⋮
-        └──YYYY_MM_DD-HH_MM_SS
-           └checkpoint.p
+    The checkpoint path can be specified directly via `path` or else it is
+    assumed to be `{project_dir}/{model_name}/checkpoint.h5`.
 
     Parameters
     ----------
-    project_dir: str
+    project_dir: str, default=None
+        Project directory; used in conjunction with `model_name` to determine the
+        checkpoint path if `path` is not specified.
+
+    model_name: str, default=None
+        Model name; used in conjunction with `project_dir` to determine the
+        checkpoint path if `path` is not specified.
+
+    path: str, default=None
+        Checkpoint path; if not specified, the checkpoint path is set to
+        `{project_dir}/{model_name}/checkpoint.h5`.
+
+    iteration: int, default=None
+        Determines which model snapshot to load. If None, the last snapshot is
+        loaded.
 
     Returns
     -------
-    checkpoint: dict
-        (See :py:func:`keypoint_moseq.io.load_checkpoint`)
-    """ 
-    pattern = re.compile(r'(\d{4}_\d{1,2}_\d{1,2}-\d{2}_\d{2}_\d{2})')
-    paths = list(filter(lambda p: pattern.search(p), os.listdir(project_dir)))
-    assert len(paths)>0, fill(
-        f'There are no directories in {project_dir} that contain'
-        ' a date string with format %Y_%m_%d-%H_%M_%S')
-    
-    name = sorted(
-        paths, key=lambda p: datetime.strptime(
-        pattern.search(p).group(), '%Y_%m_%d-%H_%M_%S')
-    )[-1]
-    
-    path = os.path.join(project_dir,name,'checkpoint.p')
-    return load_checkpoint(path=path), name
+    model: dict
+        Model dictionary containing states, parameters, hyperparameters,
+        noise prior, and random seed.
+
+    data: dict
+        Data dictionary containing observations, confidences, mask and
+        associated metadata (see :py:func:`keypoint_moseq.util.format_data`).
 
-
-def load_checkpoint(project_dir=None, name=None, path=None):
+    iteration: int
+        Iteration of model fitting corresponding to the loaded snapshot.
     """
-    Load model fitting checkpoint.
+    path = _get_path(project_dir, model_name, path, "checkpoint.h5")
 
-    The checkpoint path can be specified directly via `path`.
-    Othewise is assumed to be `{project_dir}/<name>/checkpoint.p`.
+    with h5py.File(path, "r") as f:
+        saved_iterations = np.sort([int(i) for i in f["model_snapshots"]])
+
+    if iteration is None:
+        iteration = saved_iterations[-1]
+    else:
+        assert iteration in saved_iterations, fill(
+            f"No snapshot found for iteration {iteration}. "
+            f"Available iterations are {saved_iterations}"
+        )
+
+    model = load_hdf5(path, f"model_snapshots/{iteration}")
+    metadata = load_hdf5(path, "metadata")
+    data = load_hdf5(path, "data")
+    return model, data, metadata, iteration
+
+
+def reindex_syllables_in_checkpoint(
+    project_dir=None, model_name=None, path=None, index=None, runlength=True
+):
+    """Reindex syllable labels by their frequency in the most recent model
+    snapshot in a checkpoint file.
+
+    This is an in-place operation: the checkpoint is loaded from disk, modified
+    and saved to disk again. The label permutation is applied to all model
+    snapshots in the checkpoint.
+
+    The checkpoint path can be specified directly via `path` or else it is
+    assumed to be `{project_dir}/{model_name}/checkpoint.h5`.
 
     Parameters
     ----------
     project_dir: str, default=None
-    name: str, default=None
+    model_name: str, default=None
     path: str, default=None
 
+    index: array of shape (num_states,), default=None
+        Permutation for syllable labels, where `index[i]` is relabled as `i`.
+        If None, syllables are relabled by frequency, with the most frequent
+        syllable relabled as 0, and so on.
+
+    runlength: bool, default=True
+        If True, frequencies are quantified using the number of non-consecutive
+        occurrences of each syllable. If False, frequency is quantified by
+        total number of frames.
+
     Returns
     -------
-    checkpoint: dict
-        See :py:func:`keypoint_moseq.io.save_checkpoint`
-    """
-    if path is None: 
-        assert project_dir is not None and name is not None, fill(
-            '`name` and `project_dir` are required if no `path` is given.')
-        path = os.path.join(project_dir,name,'checkpoint.p')
-    return joblib.load(path)
-
-
-def save_checkpoint(model, data, history, labels, iteration, 
-                    path=None, name=None, project_dir=None,
-                    save_history=True, save_states=True, save_data=True):
-    """
-    Save a checkpoint during model fitting.
-
-    A single checkpoint file contains model snapshots from the full history
-    of model fitting. To restart fitting from an iteration earlier than the
-    last iteration, use :py:func:`keypoint_moseq.fitting.revert`.
-
-    The checkpoint path can be specified directly via `path`.
-    Otherwise is assumed to be `{project_dir}/<name>/checkpoint.p`. See
-    :py:func:`keypoint_moseq.fitting.fit_model` for a more detailed
-    description of the checkpoint contents.
+    index: array of shape (num_states,)
+        The index used for permuting syllable labels. If `index[i] = j`, then
+        the syllable formerly labeled `j` is now labeled `i`.
+    """
+    path = _get_path(project_dir, model_name, path, "checkpoint.h5")
+
+    with h5py.File(path, "r") as f:
+        saved_iterations = [int(i) for i in f["model_snapshots"]]
+
+    if index is None:
+        with h5py.File(path, "r") as f:
+            last_iter = np.max(saved_iterations)
+            num_states = f[f"model_snapshots/{last_iter}/params/pi"].shape[0]
+            z = f[f"model_snapshots/{last_iter}/states/z"][()]
+            mask = f["data/mask"][()]
+        index = np.argsort(get_frequencies(z, mask, num_states, runlength))[
+            ::-1
+        ]
+
+    def _reindex(model):
+        model["params"]["betas"] = model["params"]["betas"][index]
+        model["params"]["pi"] = model["params"]["pi"][index, :][:, index]
+        model["params"]["Ab"] = model["params"]["Ab"][index]
+        model["params"]["Q"] = model["params"]["Q"][index]
+        model["states"]["z"] = np.argsort(index)[model["states"]["z"]]
+        return model
+
+    for iteration in tqdm.tqdm(
+        saved_iterations, desc="Reindexing", unit="model snapshot", ncols=72
+    ):
+        model = load_hdf5(path, f"model_snapshots/{iteration}")
+        save_hdf5(path, _reindex(model), f"model_snapshots/{iteration}")
+    return index
+
+
+def extract_results(
+    model,
+    metadata,
+    project_dir=None,
+    model_name=None,
+    save_results=True,
+    path=None,
+):
+    """Extract model outputs and [optionally] save them to disk.
+
+    Model outputs are saved to disk as a .h5 file, either at `path`
+    if it is specified, or at `{project_dir}/{model_name}/results.h5` if it is not.
+    If a .h5 file with the given path already exists, the outputs will be added
+    to it. The results have the following structure::
+
+        results.h5
+        ├──recording_name1
+        │  ├──syllable      # model state sequence (z), shape=(T,)
+        │  ├──latent_state  # model latent state (x), shape=(T,latent_dim)
+        │  ├──centroid      # model centroid (v), shape=(T,dim)
+        │  └──heading       # model heading (h), shape=(T,)
+        ⋮
 
     Parameters
     ----------
-    model: dict, history: dict
-        See :py:func:`keypoint_moseq.fitting.fit_model`
-
-    data: dict, labels: list of tuples
-        See :py:func:`keypoint_moseq.io.format_data`
+    model : dict
+        Model dictionary containing states, parameters, hyperparameters,
+        noise prior, and random seed.
+
+    metadata: tuple (keys, bounds)
+        Recordings and start/end frames for the data (see
+        :py:func:`keypoint_moseq.io.format_data`).
+
+    save_results : bool, default=True
+        If True, the model outputs will be saved to disk.
+
+    project_dir : str, default=None
+        Path to the project directory. Required if `save_results=True` and
+        `results_path=None`.
+
+    model_name : str, default=None
+        Name of the model. Required if `save_results=True` and
+        `results_path=None`.
 
-    iteration: int
-        Current iteration of model fitting
+    path : str, default=None
+        Optional path for saving model outputs.
 
-    save_history: bool, default=True
-        Whether to include `history` in the checkpoint
-
-    save_states: bool, default=True
-        Whether to include `states` in the checkpoint
+    Returns
+    -------
+    results_dict : dict
+        Dictionary of model outputs with the same structure as the results
+        `.h5` file.
+    """
+    if save_results:
+        path = _get_path(project_dir, model_name, path, "results.h5")
+
+    states = jax.device_get(model["states"])
+    keys, bounds = metadata
+
+    # extract syllables; repeat first syllable an extra `nlags` times
+    nlags = states["x"].shape[1] - states["z"].shape[1]
+    syllables = unbatch(states["z"], keys, bounds + np.array([nlags, 0]))
+    syllables = {
+        k: np.pad(z[nlags:], (nlags, 0), mode="edge")
+        for k, z in syllables.items()
+    }
 
-    save_data: bool, default=True
-        Whether to include `Y`, `conf`, and `mask` in the checkpoint
-    
-    project_dir: str, default=None
-        Project directory; used in conjunction with `name` to determine
-        the checkpoint path if `path` is not specified.
+    # extract latent state, centroid, and heading
+    latent_state = unbatch(states["x"], keys, bounds)
+    centroid = unbatch(states["v"], keys, bounds)
+    heading = unbatch(states["h"], keys, bounds)
+
+    results_dict = {
+        recording_name: {
+            "syllable": syllables[recording_name],
+            "latent_state": latent_state[recording_name],
+            "centroid": centroid[recording_name],
+            "heading": heading[recording_name],
+        }
+        for recording_name in syllables.keys()
+    }
 
-    name: str, default=None
-        Model name; used in conjunction with `project_dir` to determine
-        the checkpoint path if `path` is not specified.
+    if save_results:
+        save_hdf5(path, results_dict)
+        print(fill(f"Saved results to {path}"))
 
-    path: str, default=None
-        Checkpoint path; if not specified, the checkpoint path is determined
-        from `project_dir` and `name`.
+    return results_dict
 
 
-    Returns
-    -------
-    checkpoint: dict
-        Dictionary containing `history`, `labels` and `name` as 
-        well as the key/value pairs from `model` and `data`.
-    """
-    
-    if path is None: 
-        assert project_dir is not None and name is not None, fill(
-            '`name` and `project_dir` are required if no `path` is given.')
-        path = os.path.join(project_dir,name,'checkpoint.p')
-
-    dirname = os.path.dirname(path)
-    if not os.path.exists(dirname): 
-        print(fill(f'Creating the directory {dirname}'))
-        os.makedirs(dirname)
-    
-    save_dict = {
-        'labels': labels,
-        'iteration' : iteration,
-        'hypparams' : jax.device_get(model['hypparams']),
-        'params'    : jax.device_get(model['params']), 
-        'seed'      : np.array(model['seed']),
-        'name'      : name}
-
-    if save_data: 
-        save_dict.update(jax.device_get(data))
-        
-    if save_states or save_data: 
-        save_dict['mask'] = np.array(data['mask'])
-        
-    if save_states: 
-        save_dict['states'] = jax.device_get(model['states'])
-        save_dict['noise_prior'] = jax.device_get(model['noise_prior'])
-        
-    if save_history:
-        save_dict['history'] = history
-        
-    joblib.dump(save_dict, path)
-    return save_dict
+def load_results(project_dir=None, model_name=None, path=None):
+    """Load the results from a modeled dataset.
 
-    
-def load_results(project_dir=None, name=None, path=None):
-    """
-    Load the results from a modeled dataset.
+    The results path can be specified directly via `path`. Otherwise it is
+    assumed to be `{project_dir}/{model_name}/results.h5`.
 
-    The results path can be specified directly via `path`. Otherwise
-    it is assumed to be `{project_dir}/<name>/results.h5`.
-    
     Parameters
     ----------
     project_dir: str, default=None
-    name: str, default=None
+    model_name: str, default=None
     path: str, default=None
 
     Returns
     -------
     results: dict
         See :py:func:`keypoint_moseq.fitting.apply_model`
     """
-    if path is None: 
-        assert project_dir is not None and name is not None, fill(
-            '`name` and `project_dir` are required if no `path` is given.')
-        path = os.path.join(project_dir,name,'results.h5')
+    path = _get_path(project_dir, model_name, path, "results.h5")
     return load_hdf5(path)
 
 
-def save_results_as_csv(project_dir=None, name=None, h5_path=None, 
-                        save_dir=None, use_bodyparts=None,
-                        path_sep='-', **kwargs):
-    """
-    Convert modeling results from h5 to csv format.
+def save_results_as_csv(
+    results, project_dir=None, model_name=None, save_dir=None, path_sep="-"
+):
+    """Save modeling results to csv format.
+
+    This function creates a directory and then saves a separate csv file for
+    each recording. The directory is created at `save_dir` if provided,
+    otherwise at `{project_dir}/{model_name}/results`.
 
-    The input h5 file is assumed to contain modeling outputs for one
-    or more recordings. This function creates a directory and then
-    saves a separate csv file for each.
-
-    The path to the input h5 file can be specified directly via
-    `results_path`. Otherwise it is assumed to be
-    `{project_dir}/{name}/results.h5`. The path to the output
-    directory can be specified directly via `save_dir`. Otherwise
-    it will be set to `{project_dir}/{name}/results`. Any files
-    already in the output directory will be overwritten.
-    
     Parameters
     ----------
-    project_dir: str, default=None
-        Project directory; required if `h5_path` or `save_dir` is not provided.
+    results: dict
+        See :py:func:`keypoint_moseq.io.extract_results`.
 
-    name: str, default=None
-        Name of the model; required if `h5_path` or `save_dir` is not provided.
+    project_dir: str, default=None
+        Project directory; required if `save_dir` is not provided.
 
-    h5_path: str, default=None
-        Path to the h5 file containing modeling results.
+    model_name: str, default=None
+        Name of the model; required if `save_dir` is not provided.
 
     save_dir: str, default=None
-        Path to the directory where the csv files will be saved.
-
-    use_bodyparts: list, default=None
-        List of bodyparts that were used for modeling. If provided,
-        will be used for the csv column names corresponding to 
-        `estimated_coordinates`. Otherwise, the bodyparts will be
-        named `bodypart0`, `bodypart1` etc.
+        Optional path to the directory where the csv files will be saved.
 
     path_sep: str, default='-'
-        If a path separator ("/" or "\") is present in the recording name, 
-        it will be replaced with `path_sep` when saving the csv file.
+        If a path separator ("/" or "\") is present in the recording name, it
+        will be replaced with `path_sep` when saving the csv file.
     """
+    save_dir = _get_path(
+        project_dir, model_name, save_dir, "results", "save_dir"
+    )
 
-    if h5_path is None:
-        assert project_dir is not None and name is not None, fill(
-            'Provide either a `h5_path` or a `project_dir` and `name`')
-        h5_path = os.path.join(project_dir, name, 'results.h5')
-
-    if save_dir is None:
-        assert project_dir is not None and name is not None, fill(
-            'Provide either a `save_dir` or a `project_dir` and `name`')
-        save_dir = os.path.join(project_dir, name, 'results')
-
-    if not os.path.exists(save_dir): 
+    if not os.path.exists(save_dir):
         os.makedirs(save_dir)
 
-    with h5py.File(h5_path, 'r') as results:
-        for key in tqdm.tqdm(results.keys(), desc='Saving to csv'):
-            column_names, data = [], []
-
-            if 'syllables_reindexed' in results[key].keys():
-                column_names.append(['syllables reindexed'])
-                data.append(results[key]['syllables_reindexed'][()].reshape(-1,1))
-
-            if 'syllables' in results[key].keys():
-                column_names.append(['syllables non-reindexed'])
-                data.append(results[key]['syllables'][()].reshape(-1,1))
-
-            if 'centroid' in results[key].keys():
-                d = results[key]['centroid'].shape[1]
-                column_names.append(['centroid x', 'centroid y', 'centroid z'][:d])
-                data.append(results[key]['centroid'][()])
-
-            if 'heading' in results[key].keys():
-                column_names.append(['heading'])
-                data.append(results[key]['heading'][()].reshape(-1,1))
-
-            if 'estimated_coordinates' in results[key].keys():
-                k,d = results[key]['estimated_coordinates'].shape[1:]
-                if use_bodyparts is None:
-                    use_bodyparts = [f'bodypart{i}' for i in range(k)]
-                for i, bp in enumerate(use_bodyparts):
-                    column_names.append([f'estimated {bp} x', f'estimated {bp} y', f'{bp} z'][:d])
-                    data.append(results[key]['estimated_coordinates'][:,i,:])
-
-            if 'latent_state' in results[key].keys():
-                latent_dim = results[key]['latent_state'].shape[1]
-                column_names.append([f'latent_state {i}' for i in range(latent_dim)])
-                data.append(results[key]['latent_state'][()])
-
-            dfs = [pd.DataFrame(arr, columns=cols) for arr,cols in zip(data,column_names)]
-            df = pd.concat(dfs, axis=1)
-
-            for col in df.select_dtypes(include=[np.floating]).columns:
-                df[col] = df[col].astype(float).round(4)
-
-            save_name = key.replace(os.path.sep, path_sep)
-            save_path = os.path.join(save_dir, save_name)
-            df.to_csv(f'{save_path}.csv', index=False)
-
+    for key in tqdm.tqdm(results.keys(), desc="Saving to csv", ncols=72):
+        column_names, data = [], []
 
+        if "syllable" in results[key].keys():
+            column_names.append(["syllable"])
+            data.append(results[key]["syllable"].reshape(-1, 1))
+
+        if "centroid" in results[key].keys():
+            d = results[key]["centroid"].shape[1]
+            column_names.append(["centroid x", "centroid y", "centroid z"][:d])
+            data.append(results[key]["centroid"])
+
+        if "heading" in results[key].keys():
+            column_names.append(["heading"])
+            data.append(results[key]["heading"].reshape(-1, 1))
+
+        if "latent_state" in results[key].keys():
+            latent_dim = results[key]["latent_state"].shape[1]
+            column_names.append(
+                [f"latent_state {i}" for i in range(latent_dim)]
+            )
+            data.append(results[key]["latent_state"])
+
+        dfs = [
+            pd.DataFrame(arr, columns=cols)
+            for arr, cols in zip(data, column_names)
+        ]
+        df = pd.concat(dfs, axis=1)
+
+        for col in df.select_dtypes(include=[np.floating]).columns:
+            df[col] = df[col].astype(float).round(4)
+
+        save_name = key.replace(os.path.sep, path_sep)
+        save_path = os.path.join(save_dir, save_name)
+        df.to_csv(f"{save_path}.csv", index=False)
 
 
 def _name_from_path(filepath, path_in_name, path_sep, remove_extension):
-    """
-    Create a name from a filepath. Either return the name of the file
-    (with the extension removed) or return the full filepath, where the
-    path separators are replaced with `path_sep`.
+    """Create a name from a filepath.
+
+    Either return the name of the file (with the extension removed) or return
+    the full filepath, where the path separators are replaced with `path_sep`.
     """
     if remove_extension:
         filepath = os.path.splitext(filepath)[0]
     if path_in_name:
         return filepath.replace(os.path.sep, path_sep)
     else:
         return os.path.basename(filepath)
 
 
-def _print_colored_table(row_labels, col_labels, values):
-    try:
-        from IPython.display import display
-        display_available = True
-    except ImportError:
-        display_available = False
-
-    title = 'Proportion of NaNs'
-    df = pd.DataFrame(values, index=row_labels, columns=col_labels)
-    
-    if display_available:
-        def colorize(val):
-            color = plt.get_cmap("Reds")(val*0.8)
-            return f'background-color: rgba({int(color[0]*255)}, {int(color[1]*255)}, {int(color[2]*255)}, {color[3]})'  
-        colored_df = df.style.applymap(colorize).set_caption('Proportion of NaNs')
-        display(colored_df)
-        return colored_df
-    else:
-        print(title)
-        print(tabulate(df, headers='keys', tablefmt="simple_grid", showindex=True))
-
-
-def check_nan_proportions(coordinates, bodyparts, 
-                          warning_threshold=0.5,
-                          breakdown=False, **kwargs):
-    """
-    Check if any bodyparts have a high proportion of NaNs.
-    
-    Parameters
-    ----------
-    coordinates: dict
-        Dictionary mapping filenames to keypoint coordinates as ndarrays
-        of shape (n_frames, n_bodyparts, 2)
-
-    bodyparts: list of str
-        Name of each bodypart. The order of the names should match the
-        order of the bodyparts in `coordinates`.
-
-    warning_threshold: float, default=0.5
-        If the proportion of NaNs for a bodypart is greater than
-        `warning_threshold`, then a warning is printed.
-        
-    breakdown: bool, default=False
-        Whether to print a table detailing the proportion of NaNs
-        for each bodyparts in each array of `coordinates`.
-    """
-    if breakdown:
-        keys = sorted(coordinates.keys())
-        nan_props = [np.isnan(coordinates[k]).any(-1).mean(0) for k in keys]
-        _print_colored_table(keys, bodyparts, nan_props)
-    else:
-        all_coords = np.concatenate(list(coordinates.values()))
-        nan_props = np.isnan(all_coords).any(-1).mean(0)
-        if np.any(nan_props > warning_threshold):
-            bps = [bp for bp,p in zip(bodyparts,nan_props) if p > warning_threshold]
-            warnings.warn(
-                 '\nCoordinates for the following bodyparts are missing (set to NaN) in at least '
-                 '{}% of frames:\n - {}\n\n'.format(warning_threshold*100, '\n - '.join(bps)))
-            warnings.warn(
-                'This may cause problems during modeling. See '
-                'https://keypoint-moseq.readthedocs.io/en/latest/FAQs.html#high-proportion-of-nans'
-                ' for additional information.')
-
-
-def load_keypoints(filepath_pattern, format, recursive=True, path_sep='-',
-                   path_in_name=False, remove_extension=True):
+def load_keypoints(
+    filepath_pattern,
+    format,
+    extension=None,
+    recursive=True,
+    path_sep="-",
+    path_in_name=False,
+    remove_extension=True,
+):
     """
     Load keypoint tracking results from one or more files. Several file
     formats are supported:
 
     - deeplabcut
         .csv and .h5/.hdf5 files generated by deeplabcut. For single-animal
-        tracking, each file yields a single key/value pair in the returned 
-        `coordinates` and `confidences` dictionaries. For multi-animal tracking, 
-        a key/vaue pair will be generated for each tracked individual. For 
-        example the file `two_mice.h5` with individuals "mouseA" and "mouseB" 
-        will yield the pair of keys `'two_mice_mouseA', 'two_mice_mouseB'`. 
+        tracking, each file yields a single key/value pair in the returned
+        `coordinates` and `confidences` dictionaries. For multi-animal tracking,
+        a key/vaue pair will be generated for each tracked individual. For
+        example the file `two_mice.h5` with individuals "mouseA" and "mouseB"
+        will yield the pair of keys `'two_mice_mouseA', 'two_mice_mouseB'`.
 
     - sleap
-        .h5/.hdf5 files generated by sleap. For single-animal tracking, each
-        file yields a single key/value pair in the returned `coordinates` and
-        `confidences` dictionaries. For multi-animal tracking, a key/vaue pair 
-        will be generated for each track. For example a single file called 
-        `two_mice.h5` will yield the pair of keys `'two_mice_track0', 
-        'two_mice_track1'`.   
+        .slp and .h5/.hdf5 files generated by sleap. For single-animal tracking,
+        each file yields a single key/value pair in the returned `coordinates`
+        and `confidences` dictionaries. For multi-animal tracking, a key/vaue
+        pair will be generated for each track. For example a single file called
+        `two_mice.h5` will yield the pair of keys `'two_mice_track0',
+        'two_mice_track1'`.
 
     - anipose
         .csv files generated by anipose. Each file should contain five columns
-        per keypoint (x,y,z,error,score), plus a last column with the frame number.
-        The `score` column is used as the keypoint confidence. 
+        per keypoint (x,y,z,error,score), plus a last column with the frame
+        number. The `score` column is used as the keypoint confidence.
 
     - sleap-anipose
-        .h5/.hdf5 files generated by sleap-anipose. Each file should contain 
-        a dataset called `'tracks'` with shape (n_frames, 1, n_keypoints, 3).
-        If there is also a `'point_scores'` dataset, it will be used as the
+        .h5/.hdf5 files generated by sleap-anipose. Each file should contain a
+        dataset called `'tracks'` with shape (n_frames, 1, n_keypoints, 3). If
+        there is also a `'point_scores'` dataset, it will be used as the
         keypoint confidence. Otherwise, the confidence will be set to 1.
 
+    - nwb
+        .nwb files (Neurodata Without Borders). Each file should contain
+        exactly one `PoseEstimation` object (for multi-animal tracking, each
+        animal should be stored in its own .nwb file). The `PoseEstimation`
+        object should contain one `PoseEstimationSeries` object for each
+        bodypart. Confidence values are optional and will be set to 1 if not
+        present.
+
     Parameters
     ----------
     filepath_pattern: str or list of str
-        Filepath pattern for a set of deeplabcut csv or hdf5 files, 
-        or a list of such patterns. Filepath patterns can be:
+        Filepath pattern for a set of deeplabcut csv or hdf5 files, or a list
+        of such patterns. Filepath patterns can be:
 
-        - single file (e.g. `/path/to/file.csv`) 
+        - single file (e.g. `/path/to/file.csv`)
         - single directory (e.g. `/path/to/dir/`)
         - set of files (e.g. `/path/to/fileprefix*`)
         - set of directories (e.g. `/path/to/dirprefix*`)
 
     format: str
-        Format of the files to load. Must be one of `'deeplabcut'`, 
-        `'sleap'`, `'anipose'`, or `'sleap-anipose'`.
+        Format of the files to load. Must be one of `deeplabcut`, `sleap`,
+        `anipose`, or `sleap-anipose`.
+
+    extension: str, default=None
+        File extension to use when searching for files. If None, then the
+        extension will be inferred from the `format` argument:
+
+        - sleap: 'h5' or 'slp'
+        - deeplabcut: 'csv' or 'h5'
+        - anipose: 'csv'
+        - sleap-anipose: 'h5'
 
     recursive: bool, default=True
         Whether to search recursively for deeplabcut csv or hdf5 files.
 
     path_in_name: bool, default=False
-        Whether to name the tracking results from each file by the path
-        to the file (True) or just the filename (False). If True, the
-        `path_sep` argument is used to separate the path components.
-        
+        Whether to name the tracking results from each file by the path to the
+        file (True) or just the filename (False). If True, the `path_sep`
+        argument is used to separate the path components.
+
     path_sep: str, default='-'
-        Separator to use when `path_in_name` is True. For example,
-        if `path_sep` is `'-'`, then the tracking results from the
-        file `/path/to/file.csv` will be named `path-to-file`. Using
-        `'/'` as the separator is discouraged, as it will cause problems
-        saving/loading the modeling results to/from hdf5 files.
+        Separator to use when `path_in_name` is True. For example, if
+        `path_sep` is `'-'`, then the tracking results from the file
+        `/path/to/file.csv` will be named `path-to-file`. Using `'/'` as the
+        separator is discouraged, as it will cause problems saving/loading the
+        modeling results to/from hdf5 files.
 
     remove_extension: bool, default=True
-        Whether to remove the file extension when naming the tracking
-        results from each file.
+        Whether to remove the file extension when naming the tracking results
+        from each file.
 
     Returns
     -------
     coordinates: dict
-        Dictionary mapping filenames to keypoint coordinates as ndarrays
-        of shape (n_frames, n_bodyparts, 2[or 3])
+        Dictionary mapping filenames to keypoint coordinates as ndarrays of
+        shape (n_frames, n_bodyparts, 2[or 3])
 
     confidences: dict
-        Dictionary mapping filenames to `likelihood` scores as ndarrays
-        of shape (n_frames, n_bodyparts)
+        Dictionary mapping filenames to `likelihood` scores as ndarrays of
+        shape (n_frames, n_bodyparts)
 
     bodyparts: list of str
-        List of bodypart names. The order of the names matches the order
-        of the bodyparts in `coordinates` and `confidences`.
+        List of bodypart names. The order of the names matches the order of the
+        bodyparts in `coordinates` and `confidences`.
     """
-    formats = ['deeplabcut', 'sleap', 'anipose', 'sleap-anipose']
+    formats = ["deeplabcut", "sleap", "anipose", "sleap-anipose", "nwb"]
     assert format in formats, fill(
-        f'Unrecognized format {format}. Must be one of {formats}')
-    
-    extensions = {
-        'deeplabcut': ['.csv','.h5','.hdf5'],
-        'sleap': ['.h5','.hdf5'],
-        'anipose': ['.csv'],
-        'sleap-anipose': ['.h5','.hdf5']
-    }[format]
+        f"Unrecognized format {format}. Must be one of {formats}"
+    )
+
+    if extension is None:
+        extensions = {
+            "deeplabcut": [".csv", ".h5", ".hdf5"],
+            "sleap": [".h5", ".hdf5", ".slp"],
+            "anipose": [".csv"],
+            "sleap-anipose": [".h5", ".hdf5"],
+            "nwb": [".nwb"],
+        }[format]
+    else:
+        extensions = [extension]
 
     loader = {
-        'deeplabcut': _deeplabcut_loader,
-        'sleap': _sleap_loader,
-        'anipose': _anipose_loader,
-        'sleap-anipose': _sleap_anipose_loader
+        "deeplabcut": _deeplabcut_loader,
+        "sleap": _sleap_loader,
+        "anipose": _anipose_loader,
+        "sleap-anipose": _sleap_anipose_loader,
+        "nwb": _nwb_loader,
     }[format]
 
     filepaths = list_files_with_exts(
-        filepath_pattern, extensions, recursive=recursive)
-    assert len(filepaths)>0, fill(
-        f'No files with extensions {extensions} found for {filepath_pattern}')
-    
-    coordinates,confidences = {},{}
-    for filepath in tqdm.tqdm(filepaths, desc=f'Loading keypoints'):
+        filepath_pattern, extensions, recursive=recursive
+    )
+    assert len(filepaths) > 0, fill(
+        f"No files with extensions {extensions} found for {filepath_pattern}"
+    )
+
+    coordinates, confidences, bodyparts = {}, {}, None
+    for filepath in tqdm.tqdm(filepaths, desc=f"Loading keypoints", ncols=72):
         try:
-            name = _name_from_path(filepath, path_in_name, path_sep, remove_extension)
-            new_coordinates,new_confidences,bodyparts = loader(filepath, name)
-            coordinates.update(new_coordinates)
-            confidences.update(new_confidences)
+            name = _name_from_path(
+                filepath, path_in_name, path_sep, remove_extension
+            )
+            new_coordinates, new_confidences, bodyparts = loader(
+                filepath, name
+            )
+
+            if set(new_coordinates.keys()) & set(coordinates.keys()):
+                raise ValueError(
+                    fill(
+                        f"Duplicate names found in {filepath_pattern}: "
+                        f"{set(new_coordinates.keys()) & set(coordinates.keys())}. "
+                        f"Please use `path_in_name=True` to avoid this error."
+                    )
+                )
+
         except Exception as e:
-            print(fill(f'Error loading {filepath}: {e}'))
+            print(fill(f"Error loading {filepath}: {e}"))
 
-    if len(coordinates) > 0:
-        check_nan_proportions(coordinates, bodyparts)
-    return coordinates,confidences,bodyparts
+        coordinates.update(new_coordinates)
+        confidences.update(new_confidences)
+
+    assert len(coordinates) > 0, fill(
+        f"No valid results found for {filepath_pattern}"
+    )
+
+    check_nan_proportions(coordinates, bodyparts)
+    return coordinates, confidences, bodyparts
 
 
 def _deeplabcut_loader(filepath, name):
     """Load tracking results from deeplabcut csv or hdf5 files."""
     ext = os.path.splitext(filepath)[1]
-    if ext=='.h5': df = pd.read_hdf(filepath)
-    if ext=='.csv': df = pd.read_csv(filepath, header=[0,1,2], index_col=0) 
-
-    coordinates,confidences = {},{}
-    bodyparts = df.columns.get_level_values('bodyparts').unique().tolist()
-    if 'individuals' in df.columns.names:
-        for ind in df.columns.get_level_values('individuals').unique():
-            ind_df = df.xs(ind, axis=1, level='individuals')
+    if ext == ".h5":
+        df = pd.read_hdf(filepath)
+    if ext == ".csv":
+        df = pd.read_csv(filepath, header=[0, 1, 2], index_col=0)
+
+    coordinates, confidences = {}, {}
+    bodyparts = df.columns.get_level_values("bodyparts").unique().tolist()
+    if "individuals" in df.columns.names:
+        for ind in df.columns.get_level_values("individuals").unique():
+            ind_df = df.xs(ind, axis=1, level="individuals")
             arr = ind_df.to_numpy().reshape(len(ind_df), -1, 3)
-            coordinates[f'{name}_{ind}'] = arr[:,:,:-1]
-            confidences[f'{name}_{ind}'] = arr[:,:,-1]
+            coordinates[f"{name}_{ind}"] = arr[:, :, :-1]
+            confidences[f"{name}_{ind}"] = arr[:, :, -1]
     else:
         arr = df.to_numpy().reshape(len(df), -1, 3)
-        coordinates[name] = arr[:,:,:-1]
-        confidences[name] = arr[:,:,-1]
+        coordinates[name] = arr[:, :, :-1]
+        confidences[name] = arr[:, :, -1]
 
-    return coordinates,confidences,bodyparts
+    return coordinates, confidences, bodyparts
 
 
 def _sleap_loader(filepath, name):
-    """Load keypoints from sleap hdf5 files."""
-    with h5py.File(filepath, 'r') as f:
-        coords = f['tracks'][()]
-        confs = f['point_scores'][()]
-        bodyparts = [name.decode('utf-8') for name in f['node_names']]
-        if coords.shape[0] == 1: 
-            coordinates = {name: coords[0].T}
-            confidences = {name: confs[0].T}
-        else:
-            coordinates = {f'{name}_track{i}': coords[i].T for i in range(coords.shape[0])}
-            confidences = {f'{name}_track{i}': confs[i].T for i in range(coords.shape[0])}
-    return coordinates,confidences,bodyparts
+    """Load keypoints from sleap hdf5 or slp files."""
+    if os.path.splitext(filepath)[1] == ".slp":
+        slp_file = sleap_io.load_slp(filepath)
+
+        assert len(slp_file.skeletons) == 1, fill(
+            f"{filepath} contains more than one skeleton. "
+            "This is not currently supported. Please "
+            "open a github issue or email calebsw@gmail.com"
+        )
+
+        bodyparts = slp_file.skeletons[0].node_names
+        arr = slp_file.numpy(return_confidence=True)
+        coords = arr[:, :, :-1]
+        confs = arr[:, :, -1]
+    else:
+        with h5py.File(filepath, "r") as f:
+            coords = f["tracks"][()]
+            confs = f["point_scores"][()]
+            bodyparts = [name.decode("utf-8") for name in f["node_names"]]
+
+    if coords.shape[0] == 1:
+        coordinates = {name: coords[0].T}
+        confidences = {name: confs[0].T}
+    else:
+        coordinates = {
+            f"{name}_track{i}": coords[i].T for i in range(coords.shape[0])
+        }
+        confidences = {
+            f"{name}_track{i}": confs[i].T for i in range(coords.shape[0])
+        }
+    return coordinates, confidences, bodyparts
 
 
 def _anipose_loader(filepath, name):
     """Load keypoints from anipose csv files."""
-    df = pd.read_csv(filepath,)
-    bodyparts = [n.split('_x')[0] for n in df.columns[:-1][::5]] 
-    arr = df.to_numpy()[:,:-1].reshape(len(df), len(bodyparts), 5)
-    coordinates = {name: arr[:,:,:3]}
-    confidences = {name: arr[:,:,4]}
-    return coordinates,confidences,bodyparts
+    df = pd.read_csv(
+        filepath,
+    )
+    bodyparts = [n.split("_x")[0] for n in df.columns[:-1][::5]]
+    arr = df.to_numpy()[:, :-1].reshape(len(df), len(bodyparts), 5)
+    coordinates = {name: arr[:, :, :3]}
+    confidences = {name: arr[:, :, 4]}
+    return coordinates, confidences, bodyparts
 
 
 def _sleap_anipose_loader(filepath, name):
     """Load keypoints from sleap-anipose hdf5 files."""
-    with h5py.File(filepath, 'r') as f:
-        coords = f['tracks'][()]
-        if 'point_scores' in f.keys():
-            confs = f['point_scores'][()]
+    with h5py.File(filepath, "r") as f:
+        coords = f["tracks"][()]
+        if "point_scores" in f.keys():
+            confs = f["point_scores"][()]
         else:
-            confs = np.ones_like(coords[...,0])
-        bodyparts = ['bodypart{}'.format(i) for i in range(coords.shape[2])]
+            confs = np.ones_like(coords[..., 0])
+        bodyparts = ["bodypart{}".format(i) for i in range(coords.shape[2])]
         if coords.shape[1] == 1:
-            coordinates = {name: coords[:,0]}
-            confidences = {name: confs[:,0]}
+            coordinates = {name: coords[:, 0]}
+            confidences = {name: confs[:, 0]}
         else:
-            coordinates = {f'{name}_track{i}': coords[:,i] for i in range(coords.shape[1])}
-            confidences = {f'{name}_track{i}': confs[:,i] for i in range(coords.shape[1])}
-    return coordinates,confidences,bodyparts
-
-
-
-def load_deeplabcut_results(filepath_pattern, recursive=True, path_sep='-',
-                            path_in_name=False, remove_extension=True):
-    """
-    Load tracking results from deeplabcut csv or hdf5 files.
-
-    For single-animal tracking, each file yields a single key/value 
-    pair in the returned `coordinates` and `confidences` dictionaries. For
-    multi-animal tracking, a key/vaue pair will be generated for each
-    tracked individual. For example a single file called `two_mice.h5`
-    with individuals "mouseA" and "mouseB" will yield the pair of
-    keys `'two_mice_mouseA', 'two_mice_mouseB'`. 
-
-    See :py:func:`keypoint_moseq.io.load_keypoints` for a description of 
-    the parameters and return values.
-    """
-    warnings.warn(
-        'WARNING: This `load_deeplabcut_results` is being deprecated. '
-        ' Use `load_keypoints` instead.\n\n')
-    
-    filepaths = list_files_with_exts(
-        filepath_pattern, ['.csv','.h5','.hdf5'], recursive=recursive)
-    assert len(filepaths)>0, fill(
-        f'No deeplabcut csv or hdf5 files found for {filepath_pattern}')
-
-    coordinates,confidences = {},{}
-    for filepath in tqdm.tqdm(filepaths, desc='Loading from deeplabcut'):
-        
-        try:
-            ext = os.path.splitext(filepath)[1]
-            if ext=='.h5': df = pd.read_hdf(filepath)
-            if ext=='.csv': df = pd.read_csv(filepath, header=[0,1,2], index_col=0) 
-            
-            name = _name_from_path(filepath, path_in_name, path_sep, remove_extension)
-            bodyparts = df.columns.get_level_values('bodyparts').unique().tolist()   
-            
-            if 'individuals' in df.columns.names:
-                for ind in df.columns.get_level_values('individuals').unique():
-                    ind_df = df.xs(ind, axis=1, level='individuals')
-                    arr = ind_df.to_numpy().reshape(len(ind_df), -1, 3)
-                    coordinates[f'{name}_{ind}'] = arr[:,:,:-1]
-                    confidences[f'{name}_{ind}'] = arr[:,:,-1]
-            else:
-                arr = df.to_numpy().reshape(len(df), -1, 3)
-                coordinates[name] = arr[:,:,:-1]
-                confidences[name] = arr[:,:,-1]
-
-        except Exception as e: 
-            print(fill(f'Error loading {filepath}: {e}'))
-    
-    if len(coordinates) > 0:
-        check_nan_proportions(coordinates, bodyparts)
-
-    return coordinates,confidences,bodyparts
-
-
-
-def load_sleap_results(filepath_pattern, recursive=True, path_sep='-',
-                       path_in_name=False, remove_extension=True):
-    """
-    Load keypoints from sleap hdf5 files. 
-
-    For single-animal tracking, each file yields a single key/value 
-    pair in the returned `coordinates` and `confidences` dictionaries. For
-    multi-animal tracking, a key/vaue pair will be generated for each track.
-    For example a single file called `two_mice.h5` will yield the pair of
-    keys `'two_mice_track0', 'two_mice_track1'`.
-
-    See :py:func:`keypoint_moseq.io.load_keypoints` for a description of 
-    the parameters and return values.
-    """
-    warnings.warn(
-        'WARNING: This `load_sleap_results` is being deprecated. '
-        ' Use `load_keypoints` instead.\n\n')
-    
-    filepaths = list_files_with_exts(
-        filepath_pattern, ['.h5','.hdf5'], recursive=recursive)
-    assert len(filepaths)>0, fill(
-        f'No sleap hdf5 files found for {filepath_pattern}.')
-
-    coordinates,confidences = {},{}
-    for filepath in tqdm.tqdm(filepaths, desc='Loading from sleap'):
-        try: 
-            name = _name_from_path(filepath, path_in_name, path_sep, remove_extension)
-            with h5py.File(filepath, 'r') as f:
-                coords = f['tracks'][()]
-                confs = f['point_scores'][()]
-                bodyparts = [name.decode('utf-8') for name in f['node_names']]
-                if coords.shape[0] == 1: 
-                    coordinates[name] = coords[0].T
-                    confidences[name] = confs[0].T
-                else:
-                    for i in range(coords.shape[0]):
-                        coordinates[f'{name}_track{i}'] = coords[i].T
-                        confidences[f'{name}_track{i}'] = confs[i].T
-        except Exception as e: 
-            print(fill(f'Error loading {filepath}: {e}'))
-
-    if len(coordinates) > 0:
-        check_nan_proportions(coordinates, bodyparts)
-
-    return coordinates,confidences,bodyparts
-
-
-
-
-
-
-
+            coordinates = {
+                f"{name}_track{i}": coords[:, i]
+                for i in range(coords.shape[1])
+            }
+            confidences = {
+                f"{name}_track{i}": confs[:, i] for i in range(coords.shape[1])
+            }
+    return coordinates, confidences, bodyparts
+
+
+def _load_nwb_pose_obj(io, filepath):
+    """Grab PoseEstimation object from an opened .nwb file."""
+    all_objs = io.read().all_children()
+    pose_objs = [o for o in all_objs if isinstance(o, PoseEstimation)]
+    assert len(pose_objs) > 0, fill(
+        f"No PoseEstimation objects found in {filepath}"
+    )
+    assert len(pose_objs) == 1, fill(
+        f"Found multiple PoseEstimation objects in {filepath}. "
+        "This is not currently supported. Please open a github "
+        "issue to request this feature."
+    )
+    pose_obj = pose_objs[0]
+    return pose_obj
+
+
+def _nwb_loader(filepath, name):
+    """Load keypoints from nwb files."""
+    with NWBHDF5IO(filepath, mode="r", load_namespaces=True) as io:
+        pose_obj = _load_nwb_pose_obj(io, filepath)
+        bodyparts = list(pose_obj.nodes[:])
+        coords = np.stack(
+            [pose_obj.pose_estimation_series[bp].data[()] for bp in bodyparts],
+            axis=1,
+        )
+        if (
+            "confidence"
+            in pose_obj.pose_estimation_series[bodyparts[0]].fields
+        ):
+            confs = np.stack(
+                [
+                    pose_obj.pose_estimation_series[bp].confidence[()]
+                    for bp in bodyparts
+                ],
+                axis=1,
+            )
+        else:
+            confs = np.ones_like(coords[..., 0])
+        coordinates = {name: coords}
+        confidences = {name: confs}
+    return coordinates, confidences, bodyparts
 
 
+def save_hdf5(filepath, save_dict, datapath=None):
+    """Save a dict of pytrees to an hdf5 file. The leaves of the pytrees must
+    be numpy arrays, scalars, or strings.
 
-# hdf5 save/load routines modified from
-# https://gist.github.com/nirum/b119bbbd32d22facee3071210e08ecdf
-def save_hdf5(filepath, save_dict):
-    """
-    Save a dict of pytrees to an hdf5 file.
-    
     Parameters
     ----------
     filepath: str
         Path of the hdf5 file to create.
 
     save_dict: dict
-        Dictionary where the values are pytrees, i.e. recursive 
-        collections of tuples, lists, dicts, and numpy arrays.
-    """
-    with h5py.File(filepath, 'a') as f:
-        for k,tree in save_dict.items():
-            _savetree_hdf5(jax.device_get(tree), f, k)
+        Dictionary where the values are pytrees, i.e. recursive collections of
+        tuples, lists, dicts, and numpy arrays.
+
+    datapath: str, default=None
+        Path within the hdf5 file to save the data. If None, the data is saved
+        at the root of the hdf5 file.
+    """
+    with h5py.File(filepath, "a") as f:
+        if datapath is not None:
+            _savetree_hdf5(jax.device_get(save_dict), f, datapath)
+        else:
+            for k, tree in save_dict.items():
+                _savetree_hdf5(jax.device_get(tree), f, k)
 
-def load_hdf5(filepath):
-    """
-    Load a dict of pytrees from an hdf5 file.
+
+def load_hdf5(filepath, datapath=None):
+    """Load a dict of pytrees from an hdf5 file.
 
     Parameters
     ----------
     filepath: str
         Path of the hdf5 file to load.
-            
+
+    datapath: str, default=None
+        Path within the hdf5 file to load the data from. If None, the data is
+        loaded from the root of the hdf5 file.
+
     Returns
     -------
     save_dict: dict
-        Dictionary where the values are pytrees, i.e. recursive
-        collections of tuples, lists, dicts, and numpy arrays.
+        Dictionary where the values are pytrees, i.e. recursive collections of
+        tuples, lists, dicts, and numpy arrays.
     """
-    with h5py.File(filepath, 'r') as f:
-        return {k:_loadtree_hdf5(f[k]) for k in f}
+    with h5py.File(filepath, "r") as f:
+        if datapath is None:
+            return {k: _loadtree_hdf5(f[k]) for k in f}
+        else:
+            return _loadtree_hdf5(f[datapath])
+
 
 def _savetree_hdf5(tree, group, name):
     """Recursively save a pytree to an h5 file group."""
-    if name in group: del group[name]
+    if name in group:
+        del group[name]
     if isinstance(tree, np.ndarray):
+        if tree.dtype.kind == "U":
+            dt = h5py.special_dtype(vlen=str)
+            group.create_dataset(name, data=tree.astype(object), dtype=dt)
+        else:
+            group.create_dataset(name, data=tree)
+    elif isinstance(tree, (float, int, str)):
         group.create_dataset(name, data=tree)
     else:
         subgroup = group.create_group(name)
-        subgroup.attrs['type'] = type(tree).__name__
-        if isinstance(tree, tuple) or isinstance(tree, list):
+        subgroup.attrs["type"] = type(tree).__name__
+
+        if isinstance(tree, (tuple, list)):
             for k, subtree in enumerate(tree):
-                _savetree_hdf5(subtree, subgroup, f'arr{k}')
+                _savetree_hdf5(subtree, subgroup, f"arr{k}")
         elif isinstance(tree, dict):
             for k, subtree in tree.items():
                 _savetree_hdf5(subtree, subgroup, k)
-        else: raise ValueError(f'Unrecognized type {type(tree)}')
+        else:
+            raise ValueError(f"Unrecognized type {type(tree)}")
+
 
 def _loadtree_hdf5(leaf):
     """Recursively load a pytree from an h5 file group."""
     if isinstance(leaf, h5py.Dataset):
-        return np.array(leaf)
+        data = np.array(leaf[()])
+        if h5py.check_dtype(vlen=data.dtype) == str:
+            data = np.array([item.decode("utf-8") for item in data])
+        elif data.dtype.kind == "S":
+            data = data.item().decode("utf-8")
+        elif data.shape == ():
+            data = data.item()
+        return data
     else:
-        leaf_type = leaf.attrs['type']
+        leaf_type = leaf.attrs["type"]
         values = map(_loadtree_hdf5, leaf.values())
-        if leaf_type == 'dict': return dict(zip(leaf.keys(), values))
-        elif leaf_type == 'list': return list(values)
-        elif leaf_type == 'tuple': return tuple(values)
-        else: raise ValueError(f'Unrecognized type {leaf_type}')
-
+        if leaf_type == "dict":
+            return dict(zip(leaf.keys(), values))
+        elif leaf_type == "list":
+            return list(values)
+        elif leaf_type == "tuple":
+            return tuple(values)
+        else:
+            raise ValueError(f"Unrecognized type {leaf_type}")
```

### Comparing `keypoint-moseq-0.1.5/keypoint_moseq/viz.py` & `keypoint-moseq-0.2.0/keypoint_moseq/viz.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,501 +1,600 @@
 import os
 import cv2
 import tqdm
 import imageio
 import warnings
 import logging
+import h5py
 import numpy as np
+import plotly
 import matplotlib.pyplot as plt
 from scipy.ndimage import gaussian_filter1d
 from vidio.read import OpenCVReader
+from scipy.spatial.distance import squareform
+from scipy.cluster.hierarchy import linkage, dendrogram
 from textwrap import fill
 from PIL import Image
-plt.rcParams['figure.dpi'] = 100
-
-from keypoint_moseq.util import (
-    get_edges, get_durations, get_frequencies, reindex_by_bodyparts,
-    find_matching_videos, get_syllable_instances, sample_instances,
-    filter_centroids_headings, get_trajectories, interpolate_keypoints,
-    interpolate_along_axis
-)
-from keypoint_moseq.io import load_results
+from keypoint_moseq.util import *
+from keypoint_moseq.io import load_results, _get_path
 from jax_moseq.models.keypoint_slds import center_embedding
+from jax_moseq.utils import get_durations, get_frequencies
 
+# set matplotlib defaults
+plt.rcParams["figure.dpi"] = 100
 
 # suppress warnings from imageio
 logging.getLogger().setLevel(logging.ERROR)
 
 
 def crop_image(image, centroid, crop_size):
-    """
-    Crop an image around a centroid.
+    """Crop an image around a centroid.
 
     Parameters
     ----------
     image: ndarray of shape (height, width, 3)
         Image to crop.
 
     centroid: tuple of int
         (x,y) coordinates of the centroid.
 
     crop_size: int or tuple(int,int)
-        Size of the crop around the centroid. Either a single int for
-        a square crop, or a tuple of ints (w,h) for a rectangular crop.
+        Size of the crop around the centroid. Either a single int for a square
+        crop, or a tuple of ints (w,h) for a rectangular crop.
 
 
     Returns
     -------
     image: ndarray of shape (crop_size, crop_size, 3)
         Cropped image.
     """
-    if isinstance(crop_size,tuple): w,h = crop_size
-    else: w,h = crop_size,crop_size
-    x,y = int(centroid[0]),int(centroid[1])
-
-    x_min = max(0, x - w//2)
-    y_min = max(0, y - h//2)
-    x_max = min(image.shape[1], x + w//2)
-    y_max = min(image.shape[0], y + h//2)
+    if isinstance(crop_size, tuple):
+        w, h = crop_size
+    else:
+        w, h = crop_size, crop_size
+    x, y = int(centroid[0]), int(centroid[1])
+
+    x_min = max(0, x - w // 2)
+    y_min = max(0, y - h // 2)
+    x_max = min(image.shape[1], x + w // 2)
+    y_max = min(image.shape[0], y + h // 2)
 
     cropped = image[y_min:y_max, x_min:x_max]
-    padded = np.zeros((h,w,*image.shape[2:]), dtype=image.dtype)
+    padded = np.zeros((h, w, *image.shape[2:]), dtype=image.dtype)
     pad_x = (w - cropped.shape[1]) // 2
     pad_y = (h - cropped.shape[0]) // 2
-    padded[pad_y:pad_y+cropped.shape[0], pad_x:pad_x+cropped.shape[1]] = cropped
+    padded[
+        pad_y : pad_y + cropped.shape[0], pad_x : pad_x + cropped.shape[1]
+    ] = cropped
     return padded
 
 
-def plot_scree(pca, savefig=True, project_dir=None, fig_size=(3,2)):
-    """
-    Plot explained variance as a function of the number of PCs.
+def plot_scree(pca, savefig=True, project_dir=None, fig_size=(3, 2)):
+    """Plot explained variance as a function of the number of PCs.
 
     Parameters
     ----------
     pca : :py:func:`sklearn.decomposition.PCA`
         Fitted PCA model
 
     savefig : bool, True
-        Whether to save the figure to a file. If true, the figure is 
-        saved to `{project_dir}/pca_scree.pdf`.
+        Whether to save the figure to a file. If true, the figure is saved to
+        `{project_dir}/pca_scree.pdf`.
 
     project_dir : str, default=None
         Path to the project directory. Required if `savefig` is True.
 
     fig_size : tuple, (2.5,2)
         Size of the figure in inches.
 
-    Returns 
+    Returns
     -------
     fig : :py:class:`matplotlib.figure.Figure`
         Figure handle
     """
     fig = plt.figure()
     num_pcs = len(pca.components_)
-    plt.plot(np.arange(num_pcs)+1,np.cumsum(pca.explained_variance_ratio_))
-    plt.xlabel('PCs')
-    plt.ylabel('Explained variance')
+    plt.plot(np.arange(num_pcs) + 1, np.cumsum(pca.explained_variance_ratio_))
+    plt.xlabel("PCs")
+    plt.ylabel("Explained variance")
     plt.gcf().set_size_inches(fig_size)
     plt.grid()
     plt.tight_layout()
-    
+
     if savefig:
         assert project_dir is not None, fill(
-            'The `savefig` option requires a `project_dir`')
-        plt.savefig(os.path.join(project_dir,'pca_scree.pdf'))
+            "The `savefig` option requires a `project_dir`"
+        )
+        plt.savefig(os.path.join(project_dir, "pca_scree.pdf"))
     plt.show()
     return fig
-          
-def plot_pcs(pca, *, use_bodyparts, skeleton, keypoint_colormap='autumn',
-             savefig=True, project_dir=None, scale=1, plot_n_pcs=10, 
-             axis_size=(2,1.5), ncols=5, node_size=30.0, linewidth=2.0, **kwargs):
+
+
+def plot_pcs(
+    pca,
+    *,
+    use_bodyparts,
+    skeleton,
+    keypoint_colormap="autumn",
+    savefig=True,
+    project_dir=None,
+    scale=1,
+    plot_n_pcs=10,
+    axis_size=(2, 1.5),
+    ncols=5,
+    node_size=30.0,
+    linewidth=2.0,
+    interactive=True,
+    **kwargs,
+):
     """
     Visualize the components of a fitted PCA model.
 
-    For each PC, a subplot shows the mean pose (semi-transparent) along
-    with a perturbation of the mean pose in the direction of the PC. 
+    For each PC, a subplot shows the mean pose (semi-transparent) along with a
+    perturbation of the mean pose in the direction of the PC.
 
     Parameters
     ----------
     pca : :py:func:`sklearn.decomposition.PCA`
         Fitted PCA model
 
     use_bodyparts : list of str
-        List of bodyparts to that are used in the model; used to index
-        bodypart names in the skeleton.
+        List of bodyparts to that are used in the model; used to index bodypart
+        names in the skeleton.
 
     skeleton : list
-        List of edges that define the skeleton, where each edge is a
-        pair of bodypart names.
+        List of edges that define the skeleton, where each edge is a pair of
+        bodypart names.
 
     keypoint_colormap : str
         Name of a matplotlib colormap to use for coloring the keypoints.
 
     savefig : bool, True
-        Whether to save the figure to a file. If true, the figure is
-        saved to `{project_dir}/pcs-{xy/xz/yz}.pdf` (`xz` and `yz`
-        are only included for 3D data).
+        Whether to save the figure to a file. If true, the figure is saved to
+        `{project_dir}/pcs-{xy/xz/yz}.pdf` (`xz` and `yz` are only included
+        for 3D data).
 
     project_dir : str, default=None
         Path to the project directory. Required if `savefig` is True.
 
     scale : float, default=0.5
         Scale factor for the perturbation of the mean pose.
 
     plot_n_pcs : int, default=10
-        Number of PCs to plot. 
+        Number of PCs to plot.
 
     axis_size : tuple of float, default=(2,1.5)
         Size of each subplot in inches.
 
     ncols : int, default=5
         Number of columns in the figure.
 
     node_size : float, default=30.0
         Size of the keypoints in the figure.
-        
+
     linewidth: float, default=2.0
         Width of edges in skeleton
+
+    interactive : bool, default=True
+        For 3D data, whether to generate an interactive 3D plot.
     """
     k = len(use_bodyparts)
-    d = len(pca.mean_)//(k-1)  
+    d = len(pca.mean_) // (k - 1)
     Gamma = np.array(center_embedding(k))
     edges = get_edges(use_bodyparts, skeleton)
-    cmap = plt.cm.get_cmap(keypoint_colormap)
+    cmap = plt.colormaps[keypoint_colormap]
     plot_n_pcs = min(plot_n_pcs, pca.components_.shape[0])
-    
-    if d==2: dims_list,names = [[0,1]],['xy']
-    if d==3: dims_list,names = [[0,1],[0,2]],['xy','xz']
-    
+
     magnitude = np.sqrt((pca.mean_**2).mean()) * scale
-    for dims,name in zip(dims_list,names):
-        nrows = int(np.ceil(plot_n_pcs/ncols))
-        fig,axs = plt.subplots(nrows, ncols, sharex=True, sharey=True)
-        for i,ax in enumerate(axs.flat):
+    ymean = Gamma @ pca.mean_.reshape(k - 1, d)
+    ypcs = (pca.mean_ + magnitude * pca.components_).reshape(-1, k - 1, d)
+    ypcs = Gamma[np.newaxis] @ ypcs[:plot_n_pcs]
+
+    if d == 2:
+        dims_list, names = [[0, 1]], ["xy"]
+    if d == 3:
+        dims_list, names = [[0, 1], [0, 2]], ["xy", "xz"]
+
+    for dims, name in zip(dims_list, names):
+        nrows = int(np.ceil(plot_n_pcs / ncols))
+        fig, axs = plt.subplots(nrows, ncols, sharex=True, sharey=True)
+        for i, ax in enumerate(axs.flat):
             if i >= plot_n_pcs:
-                ax.axis('off')
+                ax.axis("off")
                 continue
 
-            ymean = Gamma @ pca.mean_.reshape(k-1,d)[:,dims]
-            y = Gamma @ (pca.mean_ + magnitude*pca.components_[i]).reshape(k-1,d)[:,dims]
-            
-            for e in edges:  
-                ax.plot(*ymean[e].T, color=cmap(e[0]/(k-1)), 
-                        zorder=0, alpha=0.25, linewidth=linewidth)
-                ax.plot(*y[e].T, color='k', 
-                        zorder=2, linewidth=linewidth+.2)
-                ax.plot(*y[e].T, color=cmap(e[0]/(k-1)), 
-                        zorder=3, linewidth=linewidth)
-                
-            ax.scatter(*ymean.T, c=np.arange(k), cmap=cmap, s=node_size, 
-                       zorder=1, alpha=0.25, linewidth=0)
-            ax.scatter(*y.T, c=np.arange(k), cmap=cmap, s=node_size, 
-                       zorder=4, edgecolor='k', linewidth=0.2)
-            
-            ax.set_title(f'PC {i+1}', fontsize=10)
-            ax.set_aspect('equal')
-            ax.axis('off')
-        
-        fig.set_size_inches((axis_size[0]*ncols, axis_size[1]*nrows))
+            for e in edges:
+                ax.plot(
+                    *ymean[:, dims][e].T,
+                    color=cmap(e[0] / (k - 1)),
+                    zorder=0,
+                    alpha=0.25,
+                    linewidth=linewidth,
+                )
+                ax.plot(
+                    *ypcs[i][:, dims][e].T,
+                    color="k",
+                    zorder=2,
+                    linewidth=linewidth + 0.2,
+                )
+                ax.plot(
+                    *ypcs[i][:, dims][e].T,
+                    color=cmap(e[0] / (k - 1)),
+                    zorder=3,
+                    linewidth=linewidth,
+                )
+
+            ax.scatter(
+                *ymean[:, dims].T,
+                c=np.arange(k),
+                cmap=cmap,
+                s=node_size,
+                zorder=1,
+                alpha=0.25,
+                linewidth=0,
+            )
+            ax.scatter(
+                *ypcs[i][:, dims].T,
+                c=np.arange(k),
+                cmap=cmap,
+                s=node_size,
+                zorder=4,
+                edgecolor="k",
+                linewidth=0.2,
+            )
+
+            ax.set_title(f"PC {i+1}", fontsize=10)
+            ax.set_aspect("equal")
+            ax.axis("off")
+
+        fig.set_size_inches((axis_size[0] * ncols, axis_size[1] * nrows))
         plt.tight_layout()
-        
+
         if savefig:
             assert project_dir is not None, fill(
-                'The `savefig` option requires a `project_dir`')
-            plt.savefig(os.path.join(project_dir,f'pcs-{name}.pdf'))
+                "The `savefig` option requires a `project_dir`"
+            )
+            plt.savefig(os.path.join(project_dir, f"pcs-{name}.pdf"))
         plt.show()
-        
 
-def plot_syllable_frequencies(results=None, path=None, project_dir=None, 
-                              name=None, use_reindexed=True, minlength=10,
-                              min_frequency=0.005):
-    """
-    Plot a histogram showing the frequency of each syllable.
-    
-    Caller must provide a results dictionary, a path to a results .h5,
-    or a project directory and model name, in which case the results are
-    loaded from `{project_dir}/{name}/results.h5`.
+    if interactive and d == 3:
+        plot_pcs_3D(
+            ymean,
+            ypcs,
+            edges,
+            keypoint_colormap,
+            savefig,
+            project_dir,
+            node_size / 3,
+            linewidth * 2,
+        )
+
+
+def plot_syllable_frequencies(
+    project_dir=None,
+    model_name=None,
+    results=None,
+    path=None,
+    minlength=10,
+    min_frequency=0.005,
+):
+    """Plot a histogram showing the frequency of each syllable.
+
+    Caller must provide a results dictionary, a path to a results .h5, or a
+    project directory and model name, in which case the results are loaded
+    from `{project_dir}/{model_name}/results.h5`.
 
     Parameters
     ----------
     results : dict, default=None
         Dictionary containing modeling results for a dataset (see
-        :py:func:`keypoint_moseq.fitting.apply_model`)
+        :py:func:`keypoint_moseq.fitting.extract_results`)
+
+    model_name: str, default=None
+        Name of the model. Required to load results if `results` is None and
+        `path` is None.
 
-    name: str, default=None
-        Name of the model. Required to load results if `results` is 
-        None and `path` is None. 
-        
     project_dir: str, default=None
-        Project directory. Required to load results if `results` is 
-        None and `path` is None. 
+        Project directory. Required to load results if `results` is None and
+        `path` is None.
 
     path: str, default=None
         Path to a results file. If None, results will be loaded from
-        `{project_dir}/{name}/results.h5`.
-
-    use_reindexed: bool, default=True
-        Whether to use label syllables by their frequency rank (True) or
-        or their original label (False). When reindexing, "0"  represents
-        the most frequent syllable).
+        `{project_dir}/{model_name}/results.h5`.
 
     minlength: int, default=10
         Minimum x-axis length of the histogram.
 
     min_frequency: float, default=0.005
         Minimum frequency of syllables to include in the histogram.
 
     Returns
     -------
     fig : matplotlib.figure.Figure
         Figure containing the histogram.
-    
+
     ax : matplotlib.axes.Axes
         Axes containing the histogram.
     """
     if results is None:
-        results = load_results(path=path, name=name, project_dir=project_dir)
+        results = load_results(project_dir, model_name, path)
 
-    syllable_key = 'syllables' if not use_reindexed else 'syllables_reindexed'
-    syllables = {k:res[syllable_key] for k,res in results.items()}
+    syllables = {k: res["syllable"] for k, res in results.items()}
     frequencies = get_frequencies(syllables)
-    frequencies = frequencies[frequencies>min_frequency]
-    xmax = max(minlength, np.max(np.nonzero(frequencies>min_frequency)[0])+1)
+    frequencies = frequencies[frequencies > min_frequency]
+    xmax = max(
+        minlength, np.max(np.nonzero(frequencies > min_frequency)[0]) + 1
+    )
 
     fig, ax = plt.subplots()
-    ax.bar(range(len(frequencies)),frequencies,width=1)
-    ax.set_ylabel('probability')
-    ax.set_xlabel('syllable rank')
-    ax.set_xlim(-1,xmax+1)
-    ax.set_title('Frequency distribution')
+    ax.bar(range(len(frequencies)), frequencies, width=1)
+    ax.set_ylabel("probability")
+    ax.set_xlabel("syllable rank")
+    ax.set_xlim(-1, xmax + 1)
+    ax.set_title("Frequency distribution")
     ax.set_yticks([])
     return fig, ax
 
 
-def plot_duration_distribution(results=None, path=None, project_dir=None, 
-                               name=None, lim=None, num_bins=30, fps=None, 
-                               show_median=True):
-    """
-    Plot a histogram showing the frequency of each syllable.
-    
-    Caller must provide a results dictionary, a path to a results .h5,
-    or a project directory and model name, in which case the results are
-    loaded from `{project_dir}/{name}/results.h5`.
+def plot_duration_distribution(
+    project_dir=None,
+    model_name=None,
+    results=None,
+    path=None,
+    lim=None,
+    num_bins=30,
+    fps=None,
+    show_median=True,
+):
+    """Plot a histogram showing the frequency of each syllable.
+
+    Caller must provide a results dictionary, a path to a results .h5, or a
+    project directory and model name, in which case the results are loaded from
+    `{project_dir}/{model_name}/results.h5`.
 
     Parameters
     ----------
     results : dict, default=None
         Dictionary containing modeling results for a dataset (see
-        :py:func:`keypoint_moseq.fitting.apply_model`)
+        :py:func:`keypoint_moseq.fitting.extract_results`)
+
+    model_name: str, default=None
+        Name of the model. Required to load results if `results` is None and
+        `path` is None.
 
-    name: str, default=None
-        Name of the model. Required to load results if `results` is 
-        None and `path` is None. 
-        
     project_dir: str, default=None
-        Project directory. Required to load results if `results` is 
-        None and `path` is None. 
+        Project directory. Required to load results if `results` is None and
+        `path` is None.
 
     path: str, default=None
         Path to a results file. If None, results will be loaded from
-        `{project_dir}/{name}/results.h5`.
+        `{project_dir}/{model_name}/results.h5`.
 
     lim: tuple, default=None
-        x-axis limits as a pair of ints (in units of frames). If None,
-        the limits are set to (0, 95th-percentile).
+        x-axis limits as a pair of ints (in units of frames). If None, the
+        limits are set to (0, 95th-percentile).
 
     num_bins: int, default=30
         Number of bins in the histogram.
 
     fps: int, default=None
         Frames per second. Used to convert x-axis from frames to seconds.
 
     show_median: bool, default=True
         Whether to show the median duration as a vertical line.
 
     Returns
     -------
     fig : matplotlib.figure.Figure
         Figure containing the histogram.
-    
+
     ax : matplotlib.axes.Axes
         Axes containing the histogram.
     """
     if results is None:
-        results = load_results(path=path, name=name, project_dir=project_dir)
-        
-    syllables = {k:res['syllables'] for k,res in results.items()}
+        results = load_results(project_dir, model_name, path)
+
+    syllables = {k: res["syllable"] for k, res in results.items()}
     durations = get_durations(syllables)
-    
+
     if lim is None:
         lim = int(np.percentile(durations, 95))
-    binsize = max(int(np.floor(lim/num_bins)),1)
+    binsize = max(int(np.floor(lim / num_bins)), 1)
 
     if fps is not None:
-        durations = durations/fps
-        binsize = binsize/fps
-        lim = lim/fps
-        xlabel = 'syllable duration (s)'
+        durations = durations / fps
+        binsize = binsize / fps
+        lim = lim / fps
+        xlabel = "syllable duration (s)"
     else:
-        xlabel = 'syllable duration (frames)'
+        xlabel = "syllable duration (frames)"
 
     fig, ax = plt.subplots()
-    ax.hist(durations, range=(0,lim), bins=(int(lim/binsize)), density=True)
-    ax.set_xlim([0,lim])
+    ax.hist(durations, range=(0, lim), bins=(int(lim / binsize)), density=True)
+    ax.set_xlim([0, lim])
     ax.set_xlabel(xlabel)
-    ax.set_ylabel('probability')
-    ax.set_title('Duration distribution')
+    ax.set_ylabel("probability")
+    ax.set_title("Duration distribution")
     ax.set_yticks([])
-    if show_median: ax.axvline(np.median(durations), color='k', linestyle='--')
+    if show_median:
+        ax.axvline(np.median(durations), color="k", linestyle="--")
     return fig, ax
-        
 
-def plot_progress(model, data, history, iteration, path=None,
-                  project_dir=None, name=None, savefig=True,
-                  fig_size=None, window_size=600, min_frequency=.001, 
-                  min_histogram_length=10, **kwargs):
-    """
-    Plot the progress of the model during fitting.
+
+def plot_progress(
+    model,
+    data,
+    checkpoint_path,
+    iteration,
+    project_dir=None,
+    model_name=None,
+    path=None,
+    savefig=True,
+    fig_size=None,
+    window_size=600,
+    min_frequency=0.001,
+    min_histogram_length=10,
+):
+    """Plot the progress of the model during fitting.
 
     The figure shows the following plots:
-        - Duration distribution: 
-            The distribution of state durations for the most recent
-            iteration of the model.
+        - Duration distribution:
+            The distribution of state durations for the most recent iteration
+            of the model.
         - Frequency distribution:
-            The distribution of state frequencies for the most recent
-            iteration of the model.
+            The distribution of state frequencies for the most recent iteration
+            of the model.
         - Median duration:
             The median state duration across iterations.
         - State sequence history
-            The state sequence across iterations in a random window 
-            (a new window is selected each time the progress is plotted). 
+            The state sequence across iterations in a random window (a new
+            window is selected each time the progress is plotted).
 
     Parameters
     ----------
     model : dict
         Model dictionary containing `states`
 
     data : dict
         Data dictionary containing `mask`
 
-    history : dict
-        Dictionary mapping iteration number to saved model dictionaries
+    checkpoint_path : str
+        Path to an HDF5 file containing model checkpoints.
 
     iteration : int
         Current iteration of model fitting
 
+    project_dir : str, default=None
+        Path to the project directory. Required if `savefig` is True.
+
+    model_name : str, default=None
+        Name of the model. Required if `savefig` is True.
+
     savefig : bool, default=True
-        Whether to save the figure to a file. If true, the figure is
-        either saved to `path` or, to `{project_dir}/{name}-progress.pdf`
-        if `path` is None.
+        Whether to save the figure to a file. If true, the figure is either
+        saved to `path` or, to `{project_dir}/{model_name}-progress.pdf` if
+        `path` is None.
 
     fig_size : tuple of float, default=None
-        Size of the figure in inches. 
-        
+        Size of the figure in inches.
+
     window_size : int, default=600
         Window size for state sequence history plot.
 
     min_frequency : float, default=.001
-        Minimum frequency for including a state in the frequency 
-        distribution plot.
+        Minimum frequency for including a state in the frequency distribution
+        plot.
 
     min_histogram_length : int, default=10
         Minimum x-axis length of the frequency distribution plot.
 
-    project_dir : str, default=None
-    name : str, default=None
-    path : str, default=None
-
     Returns
     -------
     fig : matplotlib.figure.Figure
         Figure containing the plots.
 
     axs : list of matplotlib.axes.Axes
         Axes containing the plots.
     """
-    z = np.array(model['states']['z'])
-    mask = np.array(data['mask'])
-    durations = get_durations(z,mask)
-    frequencies = get_frequencies(z,mask)
-    
-    history_iters = np.array(sorted(history.keys()))
-    past_stateseqs = [history[i]['states']['z'] 
-                      for i in history_iters 
-                      if 'states' in history[i]]
-        
-    if len(past_stateseqs)>0: 
-        fig,axs = plt.subplots(1,4, gridspec_kw={'width_ratios':[1,1,1,3]})
-        if fig_size is None: fig_size=(12,2.5)
-    else: 
-        fig,axs = plt.subplots(1,2)
-        if fig_size is None: fig_size=(4,2.5)
-
-    frequencies = np.sort(frequencies[frequencies>min_frequency])[::-1]
-    xmax = max(len(frequencies),min_histogram_length)
-    axs[0].bar(range(len(frequencies)),frequencies,width=1)
-    axs[0].set_ylabel('probability')
-    axs[0].set_xlabel('syllable rank')
-    axs[0].set_xlim([-1,xmax+1])
-    axs[0].set_title('Frequency distribution')
+    z = np.array(model["states"]["z"])
+    mask = np.array(data["mask"])
+    durations = get_durations(z, mask)
+    frequencies = get_frequencies(z, mask)
+
+    with h5py.File(checkpoint_path, "r") as f:
+        saved_iterations = np.sort([int(i) for i in f["model_snapshots"]])
+
+    if len(saved_iterations) > 1:
+        fig, axs = plt.subplots(
+            1, 4, gridspec_kw={"width_ratios": [1, 1, 1, 3]}
+        )
+        if fig_size is None:
+            fig_size = (12, 2.5)
+    else:
+        fig, axs = plt.subplots(1, 2)
+        if fig_size is None:
+            fig_size = (4, 2.5)
+
+    frequencies = np.sort(frequencies[frequencies > min_frequency])[::-1]
+    xmax = max(len(frequencies), min_histogram_length)
+    axs[0].bar(range(len(frequencies)), frequencies, width=1)
+    axs[0].set_ylabel("probability")
+    axs[0].set_xlabel("syllable rank")
+    axs[0].set_xlim([-1, xmax + 1])
+    axs[0].set_title("Frequency distribution")
     axs[0].set_yticks([])
-    
+
     lim = int(np.percentile(durations, 95))
-    binsize = max(int(np.floor(lim/30)),1)
-    axs[1].hist(durations, range=(1,lim), bins=(int(lim/binsize)), density=True)
-    axs[1].set_xlim([1,lim])
-    axs[1].set_xlabel('syllable duration (frames)')
-    axs[1].set_ylabel('probability')
-    axs[1].set_title('Duration distribution')
+    binsize = max(int(np.floor(lim / 30)), 1)
+    axs[1].hist(
+        durations, range=(1, lim), bins=(int(lim / binsize)), density=True
+    )
+    axs[1].set_xlim([1, lim])
+    axs[1].set_xlabel("syllable duration (frames)")
+    axs[1].set_ylabel("probability")
+    axs[1].set_title("Duration distribution")
     axs[1].set_yticks([])
-    
-    if len(past_stateseqs)>0:
-        
-        med_durs = [np.median(get_durations(z,mask)) for z in past_stateseqs]
-        axs[2].scatter(history_iters,med_durs)
-        axs[2].set_ylim([-1,np.max(med_durs)*1.1])
-        axs[2].set_xlabel('iteration')
-        axs[2].set_ylabel('duration')
-        axs[2].set_title('Median duration')
-        
-        window_size = int(min(window_size,mask.max(0).sum()-1))
-        nz = np.stack(np.array(mask[:,window_size:]).nonzero(),axis=1)
-        batch_ix,start = nz[np.random.randint(nz.shape[0])]
-        seq_hist = np.stack([z[batch_ix,start:start+window_size] for z in past_stateseqs])
-        axs[3].imshow(seq_hist, cmap=plt.cm.jet, aspect='auto', interpolation='nearest')
-        axs[3].set_xlabel('Time (frames)')
-        axs[3].set_ylabel('Iterations')
-        axs[3].set_title('State sequence history')
-        
-        yticks = [int(y) for y in axs[3].get_yticks() if y < len(history_iters) and y > 0]
-        yticklabels = history_iters[yticks]
+
+    if len(saved_iterations) > 1:
+        window_size = int(min(window_size, mask.max(0).sum() - 1))
+        nz = np.stack(np.array(mask[:, window_size:]).nonzero(), axis=1)
+        batch_ix, start = nz[np.random.randint(nz.shape[0])]
+
+        sample_state_history = []
+        median_durations = []
+
+        for i in saved_iterations:
+            with h5py.File(checkpoint_path, "r") as f:
+                z = np.array(f[f"model_snapshots/{i}/states/z"])
+                sample_state_history.append(
+                    z[batch_ix, start : start + window_size]
+                )
+                median_durations.append(np.median(get_durations(z, mask)))
+
+        axs[2].scatter(saved_iterations, median_durations)
+        axs[2].set_ylim([-1, np.max(median_durations) * 1.1])
+        axs[2].set_xlabel("iteration")
+        axs[2].set_ylabel("duration")
+        axs[2].set_title("Median duration")
+
+        axs[3].imshow(
+            sample_state_history,
+            cmap=plt.cm.jet,
+            aspect="auto",
+            interpolation="nearest",
+        )
+        axs[3].set_xlabel("Time (frames)")
+        axs[3].set_ylabel("Iterations")
+        axs[3].set_title("State sequence history")
+
+        yticks = [
+            int(y)
+            for y in axs[3].get_yticks()
+            if y < len(saved_iterations) and y > 0
+        ]
+        yticklabels = saved_iterations[yticks]
         axs[3].set_yticks(yticks)
         axs[3].set_yticklabels(yticklabels)
 
-    title = f'Iteration {iteration}'
-    if name is not None: title = f'{name}: {title}'
-    fig.suptitle(title)        
+    title = f"Iteration {iteration}"
+    if model_name is not None:
+        title = f"{model_name}: {title}"
+    fig.suptitle(title)
     fig.set_size_inches(fig_size)
     plt.tight_layout()
-    
+
     if savefig:
-        if path is None:
-            assert name is not None and project_dir is not None, fill(
-                'The `savefig` option requires either a `path` '
-                'or a `name` and `project_dir`')
-            path = os.path.join(project_dir,name,'fitting_progress.pdf')
-        plt.savefig(path)  
+        path = _get_path(project_dir, model_name, path, "fitting_progress.pdf")
+        plt.savefig(path)
     plt.show()
+    return fig, axs
 
-    return fig,axs
 
-    
 def write_video_clip(frames, path, fps=30, quality=7):
-    """
-    Write a video clip to a file.
+    """Write a video clip to a file.
 
     Parameters
     ----------
     frames : np.ndarray
         Video frames as a 4D array of shape `(num_frames, height, width, 3)`
         or a 3D array of shape `(num_frames, height, width)`.
 
@@ -505,390 +604,607 @@
     fps : int, default=30
         Framerate of video encoding.
 
     quality : int, default=7
         Quality of video encoding.
     """
     with imageio.get_writer(
-        path, pixelformat='yuv420p', 
-        fps=fps, quality=quality) as writer:
-        for frame in frames: 
+        path, pixelformat="yuv420p", fps=fps, quality=quality
+    ) as writer:
+        for frame in frames:
             writer.append_data(frame)
 
 
-def _grid_movie_tile(key, start, end, videos, centroids, headings, 
-                     dot_color, window_size, scaled_window_size,
-                     pre, post, dot_radius):
-    
-    scale_factor = scaled_window_size/window_size
-    cs = centroids[key][start-pre:start+post]
-    h,c = headings[key][start],cs[pre]
-    r = np.float32([[np.cos(h), np.sin(h)],[-np.sin(h), np.cos(h)]])
-    c = r @ c - window_size//2
-    M = [[ np.cos(h), np.sin(h),-c[0]], [-np.sin(h), np.cos(h),-c[1]]]
-    
+def _grid_movie_tile(
+    key,
+    start,
+    end,
+    videos,
+    centroids,
+    headings,
+    dot_color,
+    window_size,
+    scaled_window_size,
+    pre,
+    post,
+    dot_radius,
+    overlay_keypoints,
+    edges,
+    coordinates,
+    plot_options,
+):
+    scale_factor = scaled_window_size / window_size
+    cs = centroids[key][start - pre : start + post]
+    h, c = headings[key][start], cs[pre]
+    r = np.float32([[np.cos(h), np.sin(h)], [-np.sin(h), np.cos(h)]])
+
     tile = []
-    frames = videos[key][start-pre:start+post]
-    for ii,(frame,c) in enumerate(zip(frames,cs)):
-        frame = cv2.warpAffine(frame,np.float32(M),(window_size,window_size))
-        frame = cv2.resize(frame, (scaled_window_size,scaled_window_size))
-        if 0 <= ii-pre <= end-start and dot_radius>0:
-            pos = tuple([int(x) for x in M@np.append(c,1)*scale_factor])
-            cv2.circle(frame, pos, dot_radius, dot_color, -1, cv2.LINE_AA)
-        tile.append(frame)  
+
+    if videos is not None:  # overlay keypoints on video frame, then transform
+        frames = videos[key][start - pre : start + post]
+        c = r @ c - window_size // 2
+        M = [[np.cos(h), np.sin(h), -c[0]], [-np.sin(h), np.cos(h), -c[1]]]
+
+        for ii, (frame, c) in enumerate(zip(frames, cs)):
+            if overlay_keypoints:
+                coords = coordinates[key][start - pre + ii]
+                frame = overlay_keypoints_on_image(
+                    frame, coords, edges=edges, **plot_options
+                )
+
+            frame = cv2.warpAffine(
+                frame, np.float32(M), (window_size, window_size)
+            )
+            frame = cv2.resize(frame, (scaled_window_size, scaled_window_size))
+            if 0 <= ii - pre <= end - start and dot_radius > 0:
+                pos = tuple(
+                    [int(x) for x in M @ np.append(c, 1) * scale_factor]
+                )
+                cv2.circle(frame, pos, dot_radius, dot_color, -1, cv2.LINE_AA)
+            tile.append(frame)
+
+    else:  # first transform keypoints, then overlay on black background
+        assert overlay_keypoints, fill(
+            "If no videos are provided, then `overlay_keypoints` must "
+            "be True. Otherwise there is nothing to show"
+        )
+        scale_factor = scaled_window_size / window_size
+        coords = coordinates[key][start - pre : start + post]
+        coords = (coords - c) @ r.T * scale_factor + scaled_window_size // 2
+        cs = (cs - c) @ r.T * scale_factor + scaled_window_size // 2
+        background = np.zeros((scaled_window_size, scaled_window_size, 3))
+        for ii, (uvs, c) in enumerate(zip(coords, cs)):
+            frame = overlay_keypoints_on_image(
+                background.copy(), uvs, edges=edges, **plot_options
+            )
+            if 0 <= ii - pre <= end - start and dot_radius > 0:
+                pos = (int(c[0]), int(c[1]))
+                cv2.circle(frame, pos, dot_radius, dot_color, -1, cv2.LINE_AA)
+            tile.append(frame)
+
     return np.stack(tile)
 
 
-def grid_movie(instances, rows, cols, videos, centroids, headings,
-               window_size, dot_color=(255,255,255), dot_radius=4,
-               pre=30, post=60, scaled_window_size=None):
-    
+def grid_movie(
+    instances,
+    rows,
+    cols,
+    videos,
+    centroids,
+    headings,
+    window_size,
+    dot_color=(255, 255, 255),
+    dot_radius=4,
+    pre=30,
+    post=60,
+    scaled_window_size=None,
+    edges=[],
+    overlay_keypoints=False,
+    coordinates=None,
+    plot_options={},
+):
     """Generate a grid movie and return it as an array of frames.
 
-    Grid movies show many instances of a syllable. Each instance
-    contains a snippet of a video, centered on the animal and synchronized
-    to the onset of the syllable. A dot appears at syllable onset and 
-    disappears at syllable offset.
+    Grid movies show many instances of a syllable. Each instance contains a
+    snippet of video (and/or keypoint-overlay) centered on the animal and
+    synchronized to the onset of the syllable. A dot appears at syllable onset
+    and disappears at syllable offset.
 
     Parameters
     ----------
     instances: list of tuples `(key, start, end)`
-        List of syllable instances to include in the grid movie,
-        where each instance is specified as a tuple with the video 
-        name, start frame and end frame. The list must have length
-        `rows*cols`. The video names must also be keys in `videos`.
-        
+        List of syllable instances to include in the grid movie, where each
+        instance is specified as a tuple with the video name, start frame and
+        end frame. The list must have length `rows*cols`. The video names must
+        also be keys in `videos`.
+
     rows: int, cols : int
         Number of rows and columns in the grid movie grid
-    
-    videos: dict
+
+    videos: dict or None
         Dictionary mapping video names to video readers. Frames from
-        each reader should be accessible via `__getitem__(int or slice)`
+        each reader should be accessible via `__getitem__(int or slice)`. If
+        None, the the grid movie will not include video frames.
 
     centroids: dict
-        Dictionary mapping video names to arrays of shape `(n_frames, 2)`
-        with the x,y coordinates of animal centroid on each frame
+        Dictionary mapping video names to arrays of shape `(n_frames, 2)` with
+        the x,y coordinates of animal centroid on each frame
 
     headings: dict
-        Dictionary mapping video names to arrays of shape `(n_frames,)`
-        with the heading of the animal on each frame (in radians)
+        Dictionary mapping video names to arrays of shape `(n_frames,)` with
+        the heading of the animal on each frame (in radians)
 
     window_size: int
-        Size of the window around the animal. This should be a multiple
-        of 16 or imageio will complain.
+        Size of the window around the animal. This should be a multiple of 16
+        or imageio will complain.
 
     dot_color: tuple of ints, default=(255,255,255)
         RGB color of the dot indicating syllable onset and offset
 
     dot_radius: int, default=4
         Radius of the dot indicating syllable onset and offset
 
     pre: int, default=30
         Number of frames before syllable onset to include in the movie
 
     post: int, default=60
         Number of frames after syllable onset to include in the movie
 
     scaled_window_size: int, default=None
-        Window size after scaling the video. If None, the no scaling
-        is performed (i.e. `scaled_window_size = window_size`)
+        Window size after scaling the video. If None, the no scaling is
+        performed (i.e. `scaled_window_size = window_size`)
+
+    overlay_keypoints: bool, default=False
+        If True, overlay the pose skeleton on the video frames.
+
+    edges: list of tuples, default=[]
+        List of edges defining pose skeleton. Used when
+        `overlay_keypoints=True`.
+
+    coordinates: dict, default=None
+        Dictionary mapping video names to arrays of shape `(n_frames, 2)`.
+        Used when `overlay_keypoints=True`.
+
+    plot_options: dict, default={}
+        Dictionary of options to pass to `overlay_keypoints_on_image`.
+        Used when `overlay_keypoints=True`.
 
     Returns
     -------
     frames: array of shape `(post+pre, width, height, 3)`
-        Array of frames in the grid movie where:: 
+        Array of frames in the grid movie where::
 
             width = rows * scaled_window_size
             height = cols * scaled_window_size
-    """     
+    """
+    if videos is None:
+        assert overlay_keypoints, fill(
+            "If no videos are provided, then `overlay_keypoints` must "
+            "be True. Otherwise there is nothing to show"
+        )
+
     if scaled_window_size is None:
         scaled_window_size = window_size
 
     tiles = []
-    for i,(key,start,end) in enumerate(instances):
-        tiles.append(_grid_movie_tile(
-            key, start, end, videos, centroids, headings, 
-            dot_color, window_size, scaled_window_size,
-            pre, post, dot_radius))
-
-    tiles = np.stack(tiles).reshape(rows, cols, post+pre, scaled_window_size, scaled_window_size, 3)
-    frames = np.concatenate(np.concatenate(tiles,axis=2),axis=2)
+    for key, start, end in instances:
+        tiles.append(
+            _grid_movie_tile(
+                key,
+                start,
+                end,
+                videos,
+                centroids,
+                headings,
+                dot_color,
+                window_size,
+                scaled_window_size,
+                pre,
+                post,
+                dot_radius,
+                overlay_keypoints,
+                edges,
+                coordinates,
+                plot_options,
+            )
+        )
+
+    tiles = np.stack(tiles).reshape(
+        rows, cols, post + pre, scaled_window_size, scaled_window_size, 3
+    )
+    frames = np.concatenate(np.concatenate(tiles, axis=2), axis=2)
     return frames
 
 
-def get_grid_movie_window_size(sampled_instances, centroids, headings,
-                               coordinates, pre, post, pctl=90, 
-                               fudge_factor=1.1, blocksize=16):
-    """
-    Automatically determine the window size for a grid movie.
+def get_grid_movie_window_size(
+    sampled_instances,
+    centroids,
+    headings,
+    coordinates,
+    pre,
+    post,
+    pctl=90,
+    fudge_factor=1.1,
+    blocksize=16,
+):
+    """Automatically determine the window size for a grid movie.
 
     The window size is set such that across all sampled instances,
     the animal is fully visible in at least `pctl` percent of frames.
 
     Parameters
     ----------
     sampled_instances: dict
         Dictionary mapping syllables to lists of instances, where each
         instance is specified as a tuple with the video name, start frame
-        and end frame. 
+        and end frame.
 
     centroids: dict
         Dictionary mapping video names to arrays of shape `(n_frames, 2)`
         with the x,y coordinates of animal centroid on each frame
 
     headings: dict
         Dictionary mapping video names to arrays of shape `(n_frames,)`
         with the heading of the animal on each frame (in radians)
 
     coordinates: dict
-        Dictionary mapping session names to keypoint coordinates as 
-        ndarrays of shape (n_frames, n_bodyparts, 2). 
+        Dictionary mapping recording names to keypoint coordinates as
+        ndarrays of shape (n_frames, n_bodyparts, 2).
 
     pre, post: int
-        Number of frames before/after syllable onset that are included 
+        Number of frames before/after syllable onset that are included
         in the grid movies.
 
     pctl: int, default=95
         Percentile of frames in which the animal should be fully visible.
 
     fudge_factor: float, default=1.1
-        Factor by which to multiply the window size. 
+        Factor by which to multiply the window size.
 
     blocksize: int, default=16
         Window size is rounded up to the nearest multiple of `blocksize`.
     """
-    all_trajectories = get_trajectories(
-        sum(sampled_instances.values(), []), coordinates, pre=pre, 
-        post=post, centroids=centroids, headings=headings)
-    
+    all_trajectories = get_instance_trajectories(
+        sum(sampled_instances.values(), []),
+        coordinates,
+        pre=pre,
+        post=post,
+        centroids=centroids,
+        headings=headings,
+    )
+
     all_trajectories = np.concatenate(all_trajectories, axis=0)
+    all_trajectories = all_trajectories[
+        ~np.isnan(all_trajectories).all((1, 2))
+    ]
     max_distances = np.nanmax(np.abs(all_trajectories), axis=1)
     window_size = np.percentile(max_distances, pctl) * fudge_factor * 2
     window_size = int(np.ceil(window_size / blocksize) * blocksize)
     return window_size
 
 
 def generate_grid_movies(
-    results=None, output_dir=None, name=None, project_dir=None,
-    results_path=None, video_dir=None, video_paths=None, rows=4, 
-    cols=6, filter_size=9, pre=30, post=60, min_frequency=0.005, 
-    min_duration=3, dot_radius=4, dot_color=(255,255,255), quality=7,
-    window_size=None, use_reindexed=True, coordinates=None, 
-    bodyparts=None, use_bodyparts=None, sampling_options={},  
-    video_extension=None, max_video_size=1920, **kwargs):
-    
-    """
-    Generate grid movies for a modeled dataset.
+    results,
+    project_dir=None,
+    model_name=None,
+    output_dir=None,
+    video_dir=None,
+    video_paths=None,
+    rows=4,
+    cols=6,
+    filter_size=9,
+    pre=30,
+    post=60,
+    min_frequency=0.005,
+    min_duration=3,
+    dot_radius=4,
+    dot_color=(255, 255, 255),
+    quality=7,
+    window_size=None,
+    coordinates=None,
+    bodyparts=None,
+    use_bodyparts=None,
+    sampling_options={},
+    video_extension=None,
+    max_video_size=1920,
+    skeleton=[],
+    overlay_keypoints=False,
+    keypoints_only=False,
+    fps=30,
+    plot_options={},
+    use_dims=[0, 1],
+    keypoint_colormap="autumn",
+    **kwargs,
+):
+    """Generate grid movies for a modeled dataset.
 
     Grid movies show many instances of a syllable and are useful in
-    figuring out what behavior the syllable captures 
+    figuring out what behavior the syllable captures
     (see :py:func:`keypoint_moseq.viz.grid_movie`). This method
     generates a grid movie for each syllable that is used sufficiently
     often (i.e. has at least `rows*cols` instances with duration
     of at least `min_duration` and an overall frequency of at least
-    `min_frequency`). The grid movies are saved to `output_dir` if 
-    specified, or else to `{project_dir}/{name}/grid_movies`.
+    `min_frequency`). The grid movies are saved to `output_dir` if
+    specified, or else to `{project_dir}/{model_name}/grid_movies`.
 
     Parameters
     ----------
-    results: dict, default=None
+    results: dict
         Dictionary containing modeling results for a dataset (see
-        :py:func:`keypoint_moseq.fitting.apply_model`). Must have
-        the format::
+        :py:func:`keypoint_moseq.fitting.extract_results`)
 
-            {
-                session_name1: {
-                    'syllables':              array of shape (n_frames,),
-                    'syllables_reindexed':    array of shape (n_frames,),
-                    'centroid':               array of shape (n_frames, dim),
-                    'heading' :               array of shape (n_frames,), 
-                },
-                ...  
-            }
-            
-        - `syllables` is required if `use_reindexed=False`
-        - `syllables_reindexed` is required if `use_reindexed=True`
-        - `centroid` is always required
-        - `heading` is always required
+    project_dir: str, default=None
+        Project directory. Required to save grid movies if `output_dir`
+        is None.
 
-        If `results=None`, results will be loaded using either 
-        `results_path` or  `project_dir` and `name`.
+    model_name: str, default=None
+        Name of the model. Required to save grid movies if
+        `output_dir` is None.
 
     output_dir: str, default=None
         Directory where grid movies should be saved. If None, grid
-        movies will be saved to `{project_dir}/{name}/grid_movies`.
-
-    name: str, default=None
-        Name of the model. Required to load results if `results` is 
-        None and `results_path` is None. Required to save grid movies 
-        if `output_dir` is None.
-        
-    project_dir: str, default=None
-        Project directory. Required to load results if `results` is 
-        None and `results_path` is None. Required to save grid movies 
-        if `output_dir` is None.
-
-    results_path: str, default=None
-        Path to a results file. If None, results will be loaded from
-        `{project_dir}/{name}/results.h5`.
+        movies will be saved to `{project_dir}/{model_name}/grid_movies`.
 
     video_dir: str, default=None
-        Directory containing videos of the modeled data (see 
-        :py:func:`keypoint_moseq.io.find_matching_videos`). If None,
-        a dictionary of `video_paths` must be provided.
+        Directory containing videos of the modeled data (see
+        :py:func:`keypoint_moseq.io.find_matching_videos`).
+        Unless `keypoints_only=True`, either `video_dir` or
+        `video_paths` must be provided.
 
     video_paths: dict, default=None
-        Dictionary mapping session names to video paths. The session 
-        names must correspond to keys in `results['syllables']`. If
-        None, a `video_dir` must be provided.
+        Dictionary mapping recording names to video paths. The recording
+        names must correspond to keys in `results['syllables']`.
+        Unless `keypoints_only=True`, either `video_dir` or
+        `video_paths` must be provided.
 
     filter_size: int, default=9
         Size of the median filter applied to centroids and headings
 
     min_frequency: float, default=0.005
         Minimum frequency of a syllable to be included in the grid movies.
 
     min_duration: int, default=3
-        Minimum duration of a syllable instance to be included in the 
-        grid movie for that syllable. 
-
-    use_reindexed: bool, default=True
-        Whether to use label syllables by their frequency rank (True) or
-        or their original label (False). When reindexing, "0"  represents
-        the most frequent syllable).
+        Minimum duration of a syllable instance to be included in the
+        grid movie for that syllable.
 
     sampling_options: dict, default={}
         Dictionary of options for sampling syllable instances (see
         :py:func:`keypoint_moseq.util.sample_instances`).
-    
+
     coordinates: dict, default=None
-        Dictionary mapping session names to keypoint coordinates as 
-        ndarrays of shape (n_frames, n_bodyparts, 2). Required when
-        `window_size=None`, and for density-based sampling (i.e. when 
-        `sampling_options['mode']=='density'`; see 
-        :py:func:`keypoint_moseq.util.sample_instances`).
+        Dictionary mapping recording names to keypoint coordinates as
+        ndarrays of shape (n_frames, n_bodyparts, [2 or 3]). Required when
+        `window_size=None`, or `overlay_keypoints=True`, or if using
+        density-based sampling (i.e. when `sampling_options['mode']=='density'`;
+        see :py:func:`keypoint_moseq.util.sample_instances`).
 
     bodyparts: list of str, default=None
-        List of bodypart names in `coordinates`. Required when 
-        `coordinates` is provided and bodyparts were reindexed 
-        for modeling. 
+        List of bodypart names in `coordinates`. Required when `coordinates` is
+        provided and bodyparts were reindexed for modeling.
 
     use_bodyparts: list of str, default=None
-        Ordered list of bodyparts used for modeling. Required when 
-        `coordinates` is provided and bodyparts were reindexed 
-        for modeling. 
+        Ordered list of bodyparts used for modeling. Required when
+        `coordinates` is provided and bodyparts were reindexed
+        for modeling.
 
     quality: int, default=7
         Quality of the grid movies. Higher values result in higher
         quality movies but larger file sizes.
 
     rows, cols, pre, post, dot_radius, dot_color, window_size
         See :py:func:`keypoint_moseq.viz.grid_movie`
 
     video_extension: str, default=None
-        Preferred video extension (passed to :py:func:`keypoint_moseq.util.find_matching_videos`)
+        Preferred video extension (passed to
+        :py:func:`keypoint_moseq.util.find_matching_videos`)
 
     window_size: int, default=None
         Size of the window around the animal. If None, the window
         size is determined automatically based on the size of the
         animal. If provided explicitly, `window_size` should be a
         multiple of 16 or imageio will complain.
 
     max_video_size: int, default=4000
         Maximum size of the grid movie in pixels. If the grid movie
         is larger than this, it will be downsampled.
 
-        
+    skeleton: list of tuples, default=[]
+        List of tuples specifying the skeleton. Used when
+        `overlay_keypoints=True`.
+
+    overlay_keypoints: bool, default=False
+        Whether to overlay the keypoints on the grid movie.
+
+    keypoints_only: bool, default=False
+        Whether to only show the keypoints (i.e. no video frames).
+        Overrides `overlay_keypoints`. When this option is used,
+        the framerate should be explicitly specified using `fps`.
+
+    fps: int, default=30
+        Framerate of the grid movie. When `keypoints_only=False`,
+        this parameter is ignored and the framerate is determined
+        inferred from the video files.
+
+    plot_options: dict, default={}
+        Dictionary of options to pass to
+        :py:func:`keypoint_moseq.viz.overlay_keypoints_on_image`.
+
+    use_dims: pair of ints, default=[0,1]
+        Dimensions to use for plotting keypoints. Only used when
+        `overlay_keypoints=True` and the keypoints are 3D.
+
+    keypoint_colormap: str, default='autumn'
+        Colormap used to color keypoints. Used when
+        `overlay_keypoints=True`.
+
+
     See :py:func:`keypoint_moseq.viz.grid_movie` for the remaining parameters.
     """
-    assert (video_dir is not None) or (video_paths is not None), fill(
-        'You must provide either `video_dir` or `video_paths`') 
+    # check inputs
+    if not keypoints_only:
+        assert (video_dir is not None) or (video_paths is not None), fill(
+            "Either `video_dir` or `video_paths` is required unless `keypoints_only=True`"
+        )
+    elif not overlay_keypoints:
+        warnings.warn(
+            "Setting `overlay_keypoints=True` since `keypoints_only=True`"
+        )
+        overlay_keypoints = True
 
-    if window_size is None:
+    if window_size is None or overlay_keypoints:
         assert coordinates is not None, fill(
-            '`coordinates` must be provided if `window_size` is None')     
-    
-    if output_dir is None:
-        assert project_dir is not None and name is not None, fill(
-            'Either specify the `output_dir` where grid movies should '
-            'be saved or include a `project_dir` and `name`')
-        output_dir = os.path.join(project_dir,name, 'grid_movies')
-    if not os.path.exists(output_dir): os.makedirs(output_dir)
-    print(f'Writing grid movies to {output_dir}')
-    
+            "`coordinates` must be provided if `window_size` is None "
+            "or `overlay_keypoints` is True"
+        )
+
+    # prepare output directory
+    output_dir = _get_path(
+        project_dir, model_name, output_dir, "grid_movies", "output_dir"
+    )
+    if not os.path.exists(output_dir):
+        os.makedirs(output_dir)
+    print(f"Writing grid movies to {output_dir}")
+
+    # reindex coordinates if necessary
     if not (bodyparts is None or use_bodyparts is None or coordinates is None):
-        coordinates = reindex_by_bodyparts(coordinates, bodyparts, use_bodyparts)
+        coordinates = reindex_by_bodyparts(
+            coordinates, bodyparts, use_bodyparts
+        )
+
+    # get edges for plotting skeleton
+    edges = []
+    if len(skeleton) > 0 and overlay_keypoints:
+        edges = get_edges(use_bodyparts, skeleton)
 
-    if results is None: results = load_results(
-        name=name, project_dir=project_dir, path=results_path)
-    
-    if video_paths is None:
+    # load results
+    if results is None:
+        results = load_results(project_dir, model_name)
+
+    syllables = {k: v["syllable"] for k, v in results.items()}
+    centroids = {k: v["centroid"] for k, v in results.items()}
+    headings = {k: v["heading"] for k, v in results.items()}
+
+    # load video readers if necessary
+    if video_paths is None and not keypoints_only:
         video_paths = find_matching_videos(
-            results.keys(), video_dir, as_dict=True, 
-            video_extension=video_extension)
-        
-    videos = {k: OpenCVReader(path) for k,path in video_paths.items()}
-    fps = list(videos.values())[0].fps
-
-    syllable_key = 'syllables' + ('_reindexed' if use_reindexed else '')
-    syllables = {k:v[syllable_key] for k,v in results.items()}
-    centroids = {k:v['centroid'] for k,v in results.items()}
-    headings = {k:v['heading'] for k,v in results.items()}
+            results.keys(),
+            video_dir,
+            as_dict=True,
+            video_extension=video_extension,
+        )
+        videos = {k: OpenCVReader(path) for k, path in video_paths.items()}
+        fps = list(videos.values())[0].fps
+    else:
+        videos = None
 
+    # sample instances for each syllable
     syllable_instances = get_syllable_instances(
-        syllables, pre=pre, post=post, min_duration=min_duration,
-        min_frequency=min_frequency, min_instances=rows*cols)
-    
+        syllables,
+        pre=pre,
+        post=post,
+        min_duration=min_duration,
+        min_frequency=min_frequency,
+        min_instances=rows * cols,
+    )
+
     if len(syllable_instances) == 0:
-        warnings.warn(fill(
-            'No syllables with sufficient instances to make a grid movie. '
-            'This usually occurs when all frames have the same syllable label '
-            '(use `plot_syllable_frequencies` to check if this is the case)'))
+        warnings.warn(
+            fill(
+                "No syllables with sufficient instances to make a grid movie. "
+                "This usually occurs when all frames have the same syllable label "
+                "(use `plot_syllable_frequencies` to check if this is the case)"
+            )
+        )
         return
 
     sampled_instances = sample_instances(
-        syllable_instances, rows*cols, coordinates=coordinates, 
-        centroids=centroids, headings=headings, **sampling_options)
+        syllable_instances,
+        rows * cols,
+        coordinates=coordinates,
+        centroids=centroids,
+        headings=headings,
+        **sampling_options,
+    )
+
+    # if the data is 3D, pick 2 dimensions to use for plotting
+    keypoint_dimension = next(iter(centroids.values())).shape[-1]
+    if keypoint_dimension == 3:
+        ds = np.array(use_dims)
+        centroids = {k: v[:, ds] for k, v in centroids.items()}
+        if coordinates is not None:
+            coordinates = {k: v[:, :, ds] for k, v in coordinates.items()}
+
+    # smooth centroids and headings
+    centroids, headings = filter_centroids_headings(
+        centroids, headings, filter_size=filter_size
+    )
 
-    centroids,headings = filter_centroids_headings(
-        centroids, headings, filter_size=filter_size)
-    
+    # determine window size for grid movies
     if window_size is None:
         window_size = get_grid_movie_window_size(
-            sampled_instances, centroids, headings, 
-            coordinates, pre, post)
-        
-    # in practice we may need a smaller window...
-    scaled_window_size = max_video_size/max(rows,cols)
+            sampled_instances, centroids, headings, coordinates, pre, post
+        )
+
+    # possibly reduce window size to keep grid movies under max_video_size
+    scaled_window_size = max_video_size / max(rows, cols)
     scaled_window_size = int(np.floor(scaled_window_size / 16) * 16)
     scaled_window_size = min(scaled_window_size, window_size)
     scale_factor = scaled_window_size / window_size
 
     if scale_factor < 1:
-        warnings.warn('\n'+fill(
-            f'Videos will be downscaled by a factor of {scale_factor:.2f} '
-            f'so that the grid movies are under {max_video_size} pixels. '
-            'Use `max_video_size` to increase or decrease this size limit.')+'\n\n')
-        
-    for syllable,instances in tqdm.tqdm(
-        sampled_instances.items(), desc='Generating grid movies'):
-        
+        warnings.warn(
+            "\n"
+            + fill(
+                f"Videos will be downscaled by a factor of {scale_factor:.2f} "
+                f"so that the grid movies are under {max_video_size} pixels. "
+                "Use `max_video_size` to increase or decrease this size limit."
+            )
+            + "\n\n"
+        )
+
+    # add colormap to plot options
+    plot_options.update({"keypoint_colormap": keypoint_colormap})
+
+    # generate grid movies
+    for syllable, instances in tqdm.tqdm(
+        sampled_instances.items(), desc="Generating grid movies", ncols=72
+    ):
         frames = grid_movie(
-            instances, rows, cols, videos, centroids, headings,
-            window_size=window_size, scaled_window_size=scaled_window_size,
-            dot_color=dot_color, pre=pre, post=post, dot_radius=dot_radius)
+            instances,
+            rows,
+            cols,
+            videos,
+            centroids,
+            headings,
+            edges=edges,
+            window_size=window_size,
+            scaled_window_size=scaled_window_size,
+            dot_color=dot_color,
+            pre=pre,
+            post=post,
+            dot_radius=dot_radius,
+            overlay_keypoints=overlay_keypoints,
+            coordinates=coordinates,
+            plot_options=plot_options,
+        )
 
-        path = os.path.join(output_dir, f'syllable{syllable}.mp4')
+        path = os.path.join(output_dir, f"syllable{syllable}.mp4")
         write_video_clip(frames, path, fps=fps, quality=quality)
 
-        
-def get_limits(coordinates, pctl=1, blocksize=None,
-               left=0.2, right=0.2, top=0.2, bottom=0.2):
-    """
-    Get axis limits based on the coordinates of all keypoints.
+
+def get_limits(
+    coordinates,
+    pctl=1,
+    blocksize=None,
+    left=0.2,
+    right=0.2,
+    top=0.2,
+    bottom=0.2,
+):
+    """Get axis limits based on the coordinates of all keypoints.
 
     For each axis, limits are determined using the percentiles
     `pctl` and `100-pctl` and then padded by `padding`.
 
     Parameters
     ----------
     coordinates: ndarray or dict
@@ -897,68 +1213,77 @@
 
     pctl: float, default=1
         Percentile to use for determining the axis limits.
 
     blocksize: int, default=None
         Axis limits are cast to integers and padded so that the width
         and height are multiples of `blocksize`. This is useful
-        when they are used for generating cropped images for a video. 
-        
+        when they are used for generating cropped images for a video.
+
     left, right, top, bottom: float, default=0.1
         Fraction of the axis range to pad on each side.
 
     Returns
     -------
     lims: ndarray of shape (2,dim)
         Axis limits, in the format `[[xmin,ymin,...],[xmax,ymax,...]]`.
     """
     if isinstance(coordinates, dict):
-        X = np.concatenate(list(coordinates.values())).reshape(-1,2)
+        X = np.concatenate(list(coordinates.values())).reshape(-1, 2)
     else:
-        X = coordinates.reshape(-1,2)
+        X = coordinates.reshape(-1, 2)
+
+    xmin, ymin = np.nanpercentile(X, pctl, axis=0)
+    xmax, ymax = np.nanpercentile(X, 100 - pctl, axis=0)
 
-    xmin,ymin = np.nanpercentile(X, pctl, axis=0)
-    xmax,ymax = np.nanpercentile(X, 100-pctl, axis=0)
+    width = xmax - xmin
+    height = ymax - ymin
+    xmin -= width * left
+    xmax += width * right
+    ymin -= height * bottom
+    ymax += height * top
 
-    width = xmax-xmin
-    height = ymax-ymin
-    xmin -= width*left
-    xmax += width*right
-    ymin -= height*bottom
-    ymax += height*top
-
-    lims = np.array([
-        [xmin,ymin],
-        [xmax,ymax]])
+    lims = np.array([[xmin, ymin], [xmax, ymax]])
 
     if blocksize is not None:
         lims = np.round(lims)
-        padding = np.mod(lims[0]-lims[1], blocksize)/2
+        padding = np.mod(lims[0] - lims[1], blocksize) / 2
         lims[0] -= padding
         lims[1] += padding
-        lims = lims.astype(int)
-    
+        lims = np.ceil(lims).astype(int)
+
     return lims
 
+
 def rasterize_figure(fig):
     canvas = fig.canvas
     canvas.draw()
     width, height = canvas.get_width_height()
-    raster_flat = np.frombuffer(canvas.tostring_rgb(), dtype='uint8')
+    raster_flat = np.frombuffer(canvas.tostring_rgb(), dtype="uint8")
     raster = raster_flat.reshape((height, width, 3))
     return raster
 
 
-def plot_trajectories(titles, Xs, lims, edges=[], n_cols=4, invert=False, 
-                      keypoint_colormap='autumn', node_size=50, line_width=3, 
-                      alpha=0.2, num_timesteps=10, plot_width=4, overlap=(0.2,0),
-                      return_rasters=False):
-    """
-    Plot one or more pose trajectories on a common axis and return
-    the axis.
+def plot_trajectories(
+    titles,
+    Xs,
+    lims,
+    edges=[],
+    n_cols=4,
+    invert=False,
+    keypoint_colormap="autumn",
+    node_size=50,
+    line_width=3,
+    alpha=0.2,
+    num_timesteps=10,
+    plot_width=4,
+    overlap=(0.2, 0),
+    return_rasters=False,
+):
+    """Plot one or more pose trajectories on a common axis and return the axis.
 
     (See :py:func:`keypoint_moseq.viz.generate_trajectory_plots`)
 
     Parameters
     ----------
     titles: list of str
         List of titles for each trajectory plot.
@@ -967,410 +1292,416 @@
         List of pose trajectories as ndarrays of shape
         (n_frames, n_keypoints, 2).
 
     edges: list of tuples, default=[]
         List of edges, where each edge is a tuple of two integers
 
     lims: ndarray
-        Axis limits used for all the trajectory plots. The limits 
+        Axis limits used for all the trajectory plots. The limits
         should be provided as an array of shape (2,2) with the format
         `[[xmin,ymin],[xmax,ymax]]`.
 
     n_cols: int, default=4
         Number of columns in the figure (used when plotting multiple
         trajectories).
 
     invert: bool, default=False
         Determines the background color of the figure. If `True`,
         the background will be black.
 
     keypoint_colormap : str or list
-        Name of a matplotlib colormap or a list of colors as (r,b,g) 
+        Name of a matplotlib colormap or a list of colors as (r,b,g)
         tuples in the same order as as the keypoints.
 
     node_size: int, default=50
         Size of each keypoint.
 
     line_width: int, default=3
         Width of the lines connecting keypoints.
 
     alpha: float, default=0.2
         Opacity of fade-out layers.
 
     num_timesteps: int, default=10
-        Number of timesteps to plot for each trajectory. The pose 
+        Number of timesteps to plot for each trajectory. The pose
         at each timestep is determined by linearly interpolating
         between the keypoints.
 
     plot_width: int, default=4
-        Width of each trajectory plot in inches. The height  is 
-        determined by the aspect ratio of `lims`. The final figure 
+        Width of each trajectory plot in inches. The height  is
+        determined by the aspect ratio of `lims`. The final figure
         width is `fig_width * min(n_cols, len(X))`.
 
     overlap: tuple of float, default=(0.2,0)
-        Amount of overlap between each trajectory plot as a tuple 
+        Amount of overlap between each trajectory plot as a tuple
         with the format `(x_overlap, y_overlap)`. The values should
         be between 0 and 1.
-        
+
     return_rasters: bool, default=False
         Rasterize the matplotlib canvas after plotting each step of
         the trajecory. This is used to generate an animated video/gif
-        of the trajectory. 
+        of the trajectory.
 
     Returns
     -------
     fig : :py:class:`matplotlib.figure.Figure`
         Figure handle
 
     ax: matplotlib.axes.Axes
         Axis containing the trajectory plots.
     """
-    fill_color = 'k' if invert else 'w'
-    if isinstance(keypoint_colormap, list): colors = keypoint_colormap
-    else: colors = plt.cm.get_cmap(keypoint_colormap)(np.linspace(0,1,Xs[0].shape[1]))
+    fill_color = "k" if invert else "w"
+    if isinstance(keypoint_colormap, list):
+        colors = keypoint_colormap
+    else:
+        colors = plt.colormaps[keypoint_colormap](
+            np.linspace(0, 1, Xs[0].shape[1])
+        )
 
     n_cols = min(n_cols, len(Xs))
-    n_rows = np.ceil(len(Xs)/n_cols)
-    offsets = np.stack(np.meshgrid(
-        np.arange(n_cols)*np.diff(lims[:,0])*(1-overlap[0]),
-        np.arange(n_rows)*np.diff(lims[:,1])*(overlap[1]-1)
-    ),axis=-1).reshape(-1,2)[:len(Xs)]
-    
+    n_rows = np.ceil(len(Xs) / n_cols)
+    offsets = np.stack(
+        np.meshgrid(
+            np.arange(n_cols) * np.diff(lims[:, 0]) * (1 - overlap[0]),
+            np.arange(n_rows) * np.diff(lims[:, 1]) * (overlap[1] - 1),
+        ),
+        axis=-1,
+    ).reshape(-1, 2)[: len(Xs)]
+
     Xs = interpolate_along_axis(
-        np.linspace(0,Xs[0].shape[0],num_timesteps), 
-        np.arange(Xs[0].shape[0]), np.array(Xs), axis=1)
+        np.linspace(0, Xs[0].shape[0], num_timesteps),
+        np.arange(Xs[0].shape[0]),
+        np.array(Xs),
+        axis=1,
+    )
+
+    Xs = Xs + offsets[:, None, None]
+    xmin, ymin = lims[0] + offsets.min(0)
+    xmax, ymax = lims[1] + offsets.max(0)
 
-    Xs = Xs+offsets[:,None,None]
-    xmin,ymin = lims[0] + offsets.min(0)
-    xmax,ymax = lims[1] + offsets.max(0)
-    
-    fig,ax = plt.subplots(frameon=False)
+    fig, ax = plt.subplots(frameon=False)
     ax.fill_between(
-        [xmin,xmax], y1=[ymax,ymax], y2=[ymin,ymin], 
-        facecolor=fill_color, zorder=0, clip_on=False)
-    
-    title_xy = (lims * np.array([[0.5,0.1],[0.5,0.9]])).sum(0)
-    title_color = 'w' if invert else 'k'
-
-    for xy,text in zip(offsets+title_xy,titles):
-        ax.text(*xy, text, c=title_color, ha='center', 
-                va='top', zorder=Xs.shape[1]*4+4)
-        
+        [xmin, xmax],
+        y1=[ymax, ymax],
+        y2=[ymin, ymin],
+        facecolor=fill_color,
+        zorder=0,
+        clip_on=False,
+    )
+
+    title_xy = (lims * np.array([[0.5, 0.1], [0.5, 0.9]])).sum(0)
+    title_color = "w" if invert else "k"
+
+    for xy, text in zip(offsets + title_xy, titles):
+        ax.text(
+            *xy,
+            text,
+            c=title_color,
+            ha="center",
+            va="top",
+            zorder=Xs.shape[1] * 4 + 4,
+        )
+
     # final extents in axis
-    final_width = xmax-xmin
-    final_height = title_xy[1]-ymin
-    
-    fig_width = plot_width*(n_cols - (n_cols-1)*overlap[0])
-    fig_height = final_height/final_width*fig_width
+    final_width = xmax - xmin
+    final_height = title_xy[1] - ymin
+
+    fig_width = plot_width * (n_cols - (n_cols - 1) * overlap[0])
+    fig_height = final_height / final_width * fig_width
     fig.set_size_inches((fig_width, fig_height))
-        
-    ax.set_xlim(xmin,xmax)
-    ax.set_ylim(ymin,ymax)
-    ax.set_aspect('equal')
-    ax.axis('off')
+
+    ax.set_xlim(xmin, xmax)
+    ax.set_ylim(ymin, ymax)
+    ax.set_aspect("equal")
+    ax.axis("off")
     plt.tight_layout()
-        
-    rasters = [] # for making a gif
-    
+
+    rasters = []  # for making a gif
+
     for i in range(Xs.shape[1]):
-        for X,offset in zip(Xs,offsets):
-            for ii,jj in edges: 
-                ax.plot(*X[i,(ii,jj)].T, c='k', zorder=i*4, 
-                        linewidth=line_width, clip_on=False)
-        
-            for ii,jj in edges: 
-                ax.plot(*X[i,(ii,jj)].T, c=colors[ii], zorder=i*4+1, 
-                        linewidth=line_width*.9, clip_on=False)
-
-            ax.scatter(*X[i].T, c=colors, zorder=i*4+2, edgecolor='k', 
-                       linewidth=0.4, s=node_size, clip_on=False)
-        
-        if i < Xs.shape[1]-1: 
+        for X, offset in zip(Xs, offsets):
+            for ii, jj in edges:
+                ax.plot(
+                    *X[i, (ii, jj)].T,
+                    c="k",
+                    zorder=i * 4,
+                    linewidth=line_width,
+                    clip_on=False,
+                )
+
+            for ii, jj in edges:
+                ax.plot(
+                    *X[i, (ii, jj)].T,
+                    c=colors[ii],
+                    zorder=i * 4 + 1,
+                    linewidth=line_width * 0.9,
+                    clip_on=False,
+                )
+
+            ax.scatter(
+                *X[i].T,
+                c=colors,
+                zorder=i * 4 + 2,
+                edgecolor="k",
+                linewidth=0.4,
+                s=node_size,
+                clip_on=False,
+            )
+
+        if i < Xs.shape[1] - 1:
             ax.fill_between(
-                [xmin,xmax], y1=[ymax,ymax], y2=[ymin,ymin], 
-                facecolor=fill_color, alpha=alpha, zorder=i*4+3, clip_on=False)
- 
+                [xmin, xmax],
+                y1=[ymax, ymax],
+                y2=[ymin, ymin],
+                facecolor=fill_color,
+                alpha=alpha,
+                zorder=i * 4 + 3,
+                clip_on=False,
+            )
+
         if return_rasters:
-            rasters.append(rasterize_figure(fig))          
+            rasters.append(rasterize_figure(fig))
+
+    return fig, ax, rasters
 
-    return fig,ax,rasters
 
 def save_gif(image_list, gif_filename, duration=0.5):
     # Convert NumPy arrays to PIL Image objects
     pil_images = [Image.fromarray(np.uint8(img)) for img in image_list]
 
     # Save the PIL Images as an animated GIF
-    pil_images[0].save(gif_filename, save_all=True, append_images=pil_images[1:], 
-                       duration=int(duration*1000), loop=0)
-
+    pil_images[0].save(
+        gif_filename,
+        save_all=True,
+        append_images=pil_images[1:],
+        duration=int(duration * 1000),
+        loop=0,
+    )
 
 
 def generate_trajectory_plots(
-    coordinates=None, results=None, output_dir=None, name=None, 
-    project_dir=None, results_path=None, pre=5, post=15, 
-    min_frequency=0.005, min_duration=3, use_reindexed=True, 
-    use_estimated_coords=False, skeleton=[], bodyparts=None, 
-    use_bodyparts=None, num_samples=50, keypoint_colormap='autumn',
-    plot_options={}, sampling_options={'mode':'density'},
-    padding={'left':0.1, 'right':0.1, 'top':0.2, 'bottom':0.2},
-    save_individually=True, save_gifs=True, save_mp4s=False, fps=30, 
-    projection_planes=['xy','xz'], **kwargs):
+    coordinates,
+    results,
+    project_dir=None,
+    model_name=None,
+    output_dir=None,
+    pre=5,
+    post=15,
+    min_frequency=0.005,
+    min_duration=3,
+    skeleton=[],
+    bodyparts=None,
+    use_bodyparts=None,
+    keypoint_colormap="autumn",
+    plot_options={},
+    padding={"left": 0.1, "right": 0.1, "top": 0.2, "bottom": 0.2},
+    save_individually=True,
+    save_gifs=True,
+    save_mp4s=False,
+    fps=30,
+    projection_planes=["xy", "xz"],
+    interactive=True,
+    density_sample=True,
+    sampling_options={"mode": "density", "n_neighbors": 50},
+    **kwargs,
+):
     """
     Generate trajectory plots for a modeled dataset.
 
     Each trajectory plot shows a sequence of poses along the average
     trajectory through latent space associated with a given syllable.
-    A separate figure (and gif, optionally) is saved for each syllable, 
-    along with a single figure showing all syllables in a grid. The 
-    plots are saved to `{output_dir}` if it is provided, otherwise 
-    they are saved to `{project_dir}/{name}/trajectory_plots`.
+    A separate figure (and gif, optionally) is saved for each syllable,
+    along with a single figure showing all syllables in a grid. The
+    plots are saved to `{output_dir}` if it is provided, otherwise
+    they are saved to `{project_dir}/{model_name}/trajectory_plots`.
+
+    Plot-related parameters are described below. For the remaining
+    parameters see (:py:func:`keypoint_moseq.util.get_typical_trajectories`)
 
     Parameters
     ----------
-    coordinates : dict, default=None
-        Dictionary mapping session names to keypoint coordinates as 
-        ndarrays of shape (n_frames, n_bodyparts, 2). Required if
-        `use_estimated_coords=False`.
+    coordinates: dict
+        Dictionary mapping recording names to keypoint coordinates as
+        ndarrays of shape (n_frames, n_bodyparts, [2 or 3]).
 
-    results: dict, default=None
+    results: dict
         Dictionary containing modeling results for a dataset (see
-        :py:func:`keypoint_moseq.fitting.apply_model`). Must have
-        the format::
-
-            {
-                session_name1: {
-                    'syllables':              array of shape (n_frames,),
-                    'estimated_coordinates' : array of shape (n_frames, n_bodyparts, dim)
-                    'syllables_reindexed':    array of shape (n_frames,),
-                    'centroid':               array of shape (n_frames, dim),
-                    'heading' :               array of shape (n_frames,), 
-                },
-                ...  
-            }
-            
-        - `syllables` is required if `use_reindexed=False`
-        - `syllables_reindexed` is required if `use_reindexed=True`
-        - `centroid` is always required
-        - `heading` is always required
-        - `estimated_coordinates` is required if `use_estimated_coords=True`
-
-        If `results=None`, results will be loaded using either 
-        `results_path` or  `project_dir` and `name`.
-
-    output_dir: str, default=None
-        Directory where trajectory plots should be saved. If None, 
-        plots will be saved to `{project_dir}/{name}/trajectory_plots`.
-
-    name: str, default=None
-        Name of the model. Required to load results if `results` is 
-        None and `results_path` is None. Required to save trajectory
-        plots if `output_dir` is None.
+        :py:func:`keypoint_moseq.fitting.extract_results`).
 
     project_dir: str, default=None
-       Project directory. Required to load results if `results` is 
-        None and `results_path` is None. Required to save trajectory
-        plots if `output_dir` is None.
-
-    results_path: str, default=None
-        Path to a results file. If None, results will be loaded from
-        `{project_dir}/{name}/results.h5`.
+        Project directory. Required to save trajectory plots if
+        `output_dir` is None.
 
-    pre: int, default=5, post: int, default=15
-        Defines the temporal window around syllable onset for 
-        computing the average trajectory. Note that the window is 
-        independent of the actual duration of the syllable.
-
-    min_frequency: float, default=0.005
-        Minimum frequency of a syllable to plotted.
-
-    min_duration: float, default=3
-        Minimum duration of a syllable instance to be included in the
-        trajectory average.
+    model_name: str, default=None
+        Name of the model. Required to save trajectory plots if
+        `output_dir` is None.
 
-    use_reindexed: bool, default=True
-        Whether to use label syllables by their frequency rank (True) or
-        or their original label (False). When reindexing, "0"  represents
-        the most frequent syllable).
-
-    bodyparts: list of str, default=None
-        List of bodypart names in `coordinates`. 
-
-    use_bodyparts: list of str, default=None
-        Ordered list of bodyparts to include in trajectory plot.
-        If None, all bodyparts will be included.
+    output_dir: str, default=None
+        Directory where trajectory plots should be saved. If None,
+        plots will be saved to `{project_dir}/{model_name}/trajectory_plots`.
 
     skeleton : list, default=[]
         List of edges that define the skeleton, where each edge is a
         pair of bodypart names or a pair of indexes.
 
-    num_samples: int, default=50
-        Number of samples to used to compute the average trajectory.
-        Also used to set `n_neighbors` when sampling syllable instances
-        in `density` mode. 
-
     keypoint_colormap : str
         Name of a matplotlib colormap to use for coloring the keypoints.
 
     plot_options: dict, default={}
         Dictionary of options for trajectory plots (see
         :py:func:`keypoint_moseq.util.plot_trajectories`).
 
-    sampling_options: dict, default={'mode':'density'}
-        Dictionary of options for sampling syllable instances (see
-        :py:func:`keypoint_moseq.util.sample_instances`).
-        
     padding: dict, default={'left':0.1, 'right':0.1, 'top':0.2, 'bottom':0.2}
         Padding around trajectory plots. Controls the the distance
         between trajectories (when multiple are shown in one figure)
-        as well as the title offset. 
+        as well as the title offset.
 
     save_individually: bool, default=True
         If True, a separate figure is saved for each syllable (in
         addition to the grid figure).
-        
+
     save_gifs: bool, default=True
         Whether to save an animated gif of the trajectory plots.
-        
+
     save_mp4s: bool, default=False
         Whether to save videos of the trajectory plots as .mp4 files
-        
+
     fps: int, default=30
         Framerate of the videos from which keypoints were derived.
         Used to set the framerate of gifs when `save_gif=True`.
-        
+
     projection_planes: list (subset of ['xy', 'yz', 'xz']), default=['xy','xz']
-        For 3D data, defines the 2D plane(s) on which to project keypoint 
-        coordinates. A separate plot will be saved for each plane with 
-        the name of the plane (e.g. 'xy') as a suffix. This argument is 
+        For 3D data, defines the 2D plane(s) on which to project keypoint
+        coordinates. A separate plot will be saved for each plane with
+        the name of the plane (e.g. 'xy') as a suffix. This argument is
         ignored for 2D data.
-    """
-    if output_dir is None:
-        assert project_dir is not None and name is not None, fill(
-            'Either specify the `output_dir` where trajectory plots '
-            'should be saved or include a `project_dir` and `name`')
-        output_dir = os.path.join(project_dir,name, 'trajectory_plots')
-    if not os.path.exists(output_dir): os.makedirs(output_dir)
-    print(f'Saving trajectory plots to {output_dir}')
-        
-    if results is None: results = load_results(
-        name=name, project_dir=project_dir, path=results_path)
-
-    if use_estimated_coords:
-        coordinates = {k:v['estimated_coordinates'] for k,v in results.items()}
-    elif bodyparts is not None and use_bodyparts is not None:
-        coordinates = reindex_by_bodyparts(coordinates, bodyparts, use_bodyparts)
-
-    syllable_key = 'syllables' + ('_reindexed' if use_reindexed else '')
-    syllables = {k:v[syllable_key] for k,v in results.items()}
-    centroids = {k:v['centroid'] for k,v in results.items()}
-    headings = {k:v['heading'] for k,v in results.items()}
-    plot_options.update({'keypoint_colormap':keypoint_colormap})
-            
-    syllable_instances = get_syllable_instances(
-        syllables, pre=pre, post=post, min_duration=min_duration,
-        min_frequency=min_frequency, min_instances=num_samples)
-    
-    if len(syllable_instances) == 0:
-        warnings.warn(fill(
-            'No syllables with sufficient instances to make a trajectory plot. '
-            'This usually occurs when all frames have the same syllable label '
-            '(use `plot_syllable_frequencies` to check if this is the case)'))
-        return
-    
-    sampling_options['n_neighbors'] = num_samples
-    sampled_instances = sample_instances(
-        syllable_instances, num_samples, coordinates=coordinates, 
-        centroids=centroids, headings=headings, **sampling_options)
 
-    trajectories = {syllable: get_trajectories(
-        instances, coordinates, pre=pre, post=post, 
-        centroids=centroids, headings=headings
-        ) for syllable,instances in sampled_instances.items()}
-
-    edges = []
-    if len(skeleton)>0: 
-        if isinstance(skeleton[0][0],str):
-            assert use_bodyparts is not None, fill(
-                'If skeleton edges are specified using bodypart names, '
-                '`use_bodyparts` must be specified')
-            edges = get_edges(use_bodyparts, skeleton)
-        else: edges = skeleton
-
-    syllables = sorted(trajectories.keys())
-    titles = [f'Syllable {syllable}' for syllable in syllables]
-    Xs = np.nanmedian(np.array([trajectories[syllable] for syllable in syllables]),axis=1)  
-    
-    if Xs.shape[-1]==3:
-        projection_planes = [''.join(sorted(plane.lower())) for plane in projection_planes]
-        assert set(projection_planes) <= set(['xy','yz','xz']), fill(
-            "`projection_planes` must be a subset of `['xy','yz','xz']`")
-        all_Xs = [Xs[...,np.array({'xy':[0,1], 'yz':[1,2], 'xz':[0,2]}[plane])] for plane in projection_planes]
-        suffixes = ['.'+plane for plane in projection_planes]
-       
-    else: 
-        all_Xs = [Xs]
-        suffixes = ['']
+    interactive: bool, default=True
+        For 3D data, whether to create an visualization that can be
+        rotated and zoomed. This argument is ignored for 2D data.
+    """
+    plot_options.update({"keypoint_colormap": keypoint_colormap})
+    edges = [] if len(skeleton) == 0 else get_edges(use_bodyparts, skeleton)
+
+    output_dir = _get_path(
+        project_dir, model_name, output_dir, "grid_movies", "output_dir"
+    )
+    if not os.path.exists(output_dir):
+        os.makedirs(output_dir)
+    print(f"Saving trajectory plots to {output_dir}")
+
+    typical_trajectories = get_typical_trajectories(
+        coordinates,
+        results,
+        pre,
+        post,
+        min_frequency,
+        min_duration,
+        bodyparts,
+        use_bodyparts,
+        density_sample,
+        sampling_options,
+    )
+
+    syllable_ixs = sorted(typical_trajectories.keys())
+    titles = [f"Syllable {s}" for s in syllable_ixs]
+    Xs = np.stack([typical_trajectories[s] for s in syllable_ixs])
+
+    if Xs.shape[-1] == 3:
+        projection_planes = [
+            "".join(sorted(plane.lower())) for plane in projection_planes
+        ]
+        assert set(projection_planes) <= set(["xy", "yz", "xz"]), fill(
+            "`projection_planes` must be a subset of `['xy','yz','xz']`"
+        )
+        all_Xs = [
+            Xs[
+                ...,
+                np.array({"xy": [0, 1], "yz": [1, 2], "xz": [0, 2]}[plane]),
+            ]
+            for plane in projection_planes
+        ]
+        suffixes = ["." + plane for plane in projection_planes]
+    else:
+        all_Xs = [Xs * np.array([1, -1])]  # flip y-axis
+        suffixes = [""]
 
-    for Xs,suffix in zip(all_Xs,suffixes):
-        lims = get_limits(Xs, pctl=0, **padding)
+    for Xs_2D, suffix in zip(all_Xs, suffixes):
+        lims = get_limits(Xs_2D, pctl=0, **padding)
 
         # individual plots
         if save_individually:
-            desc = 'Generating trajectory plots'
-            for title,X in tqdm.tqdm(zip(titles,Xs), desc=desc, total=len(titles)):
-
-                fig,ax,rasters = plot_trajectories(
-                    [title], X[None], lims, edges=edges, 
+            desc = "Generating trajectory plots"
+            for title, X in tqdm.tqdm(
+                zip(titles, Xs_2D), desc=desc, total=len(titles), ncols=72
+            ):
+                fig, ax, rasters = plot_trajectories(
+                    [title],
+                    X[None],
+                    lims,
+                    edges=edges,
                     return_rasters=(save_gifs or save_mp4s),
-                    **plot_options)
+                    **plot_options,
+                )
 
-                plt.savefig(os.path.join(output_dir, f'{title}{suffix}.pdf'))
+                plt.savefig(os.path.join(output_dir, f"{title}{suffix}.pdf"))
                 plt.close(fig=fig)
 
                 if save_gifs:
-                    frame_duration = (pre+post) / len(rasters) / fps
-                    path = os.path.join(output_dir, f'{title}{suffix}.gif')
+                    frame_duration = (pre + post) / len(rasters) / fps
+                    path = os.path.join(output_dir, f"{title}{suffix}.gif")
                     save_gif(rasters, path, duration=frame_duration)
                 if save_mp4s:
-                    use_fps = len(rasters)/(pre+post)*fps
-                    path = os.path.join(output_dir, f'{title}{suffix}.mp4')
+                    use_fps = len(rasters) / (pre + post) * fps
+                    path = os.path.join(output_dir, f"{title}{suffix}.mp4")
                     write_video_clip(rasters, path, fps=use_fps)
-                    
 
         # grid plot
-        fig,ax,rasters = plot_trajectories(
-            titles, Xs, lims, edges=edges, 
+        fig, ax, rasters = plot_trajectories(
+            titles,
+            Xs_2D,
+            lims,
+            edges=edges,
             return_rasters=(save_gifs or save_mp4s),
-            **plot_options)
+            **plot_options,
+        )
 
-        plt.savefig(os.path.join(output_dir, f'all_trajectories{suffix}.pdf'))
+        plt.savefig(os.path.join(output_dir, f"all_trajectories{suffix}.pdf"))
         plt.show()
 
         if save_gifs:
-            frame_duration = (pre+post) / len(rasters) / fps
-            path = os.path.join(output_dir, f'all_trajectories{suffix}.gif')
+            frame_duration = (pre + post) / len(rasters) / fps
+            path = os.path.join(output_dir, f"all_trajectories{suffix}.gif")
             save_gif(rasters, path, duration=frame_duration)
         if save_mp4s:
-            use_fps = len(rasters)/(pre+post)*fps
-            path = os.path.join(output_dir, f'all_trajectories{suffix}.mp4')
+            use_fps = len(rasters) / (pre + post) * fps
+            path = os.path.join(output_dir, f"all_trajectories{suffix}.mp4")
             write_video_clip(rasters, path, fps=use_fps)
 
+    if interactive and Xs.shape[-1] == 3:
+        plot_trajectories_3D(Xs, titles, edges, output_dir, **plot_options)
 
 
 def overlay_keypoints_on_image(
-    image, coordinates, edges=[], keypoint_colormap='autumn',
-    node_size=2, line_width=1, copy=False, opacity=1.0):
-    """
-    Overlay keypoints on an image.
+    image,
+    coordinates,
+    edges=[],
+    keypoint_colormap="autumn",
+    node_size=2,
+    line_width=1,
+    copy=False,
+    opacity=1.0,
+):
+    """Overlay keypoints on an image.
 
     Parameters
     ----------
     image: ndarray of shape (height, width, 3)
         Image to overlay keypoints on.
-    
+
     coordinates: ndarray of shape (num_keypoints, 2)
         Array of keypoint coordinates.
 
     edges: list of tuples, default=[]
         List of edges that define the skeleton, where each edge is a
         pair of indexes.
 
@@ -1381,80 +1712,109 @@
         Size of the keypoints.
 
     line_width: int, default=2
         Width of the skeleton lines.
 
     copy: bool, default=False
         Whether to copy the image before overlaying keypoints.
-    
+
     opacity: float, default=1.0
         Opacity of the overlay graphics (0.0-1.0).
 
     Returns
     -------
     image: ndarray of shape (height, width, 3)
         Image with keypoints overlayed.
     """
-    if copy or opacity<1.0: 
+    if copy or opacity < 1.0:
         canvas = image.copy()
-    else: canvas = image
+    else:
+        canvas = image
 
-    # get colors from matplotlib and convert to 0-255 range for openc
-    colors = plt.get_cmap(keypoint_colormap)(np.linspace(0,1,coordinates.shape[0]))
-    colors = [tuple([int(c) for c in cs[:3]*255]) for cs in colors]
+    # get colors from matplotlib and convert to 0-255 range for opencv
+    colors = plt.colormaps[keypoint_colormap](
+        np.linspace(0, 1, coordinates.shape[0])
+    )
+    colors = [tuple([int(c) for c in cs[:3] * 255]) for cs in colors]
 
     # overlay skeleton
     for i, j in edges:
-        if np.isnan(coordinates[i,0]) or np.isnan(coordinates[j,0]): continue
-        pos1 = tuple(coordinates[i].astype(int))
-        pos2 = tuple(coordinates[j].astype(int))
-        canvas = cv2.line(canvas, pos1, pos2, colors[i], line_width, cv2.LINE_AA)
+        if np.isnan(coordinates[i, 0]) or np.isnan(coordinates[j, 0]):
+            continue
+        pos1 = (int(coordinates[i, 0]), int(coordinates[i, 1]))
+        pos2 = (int(coordinates[j, 0]), int(coordinates[j, 1]))
+        canvas = cv2.line(
+            canvas, pos1, pos2, colors[i], line_width, cv2.LINE_AA
+        )
 
     # overlay keypoints
-    for i, (x,y) in enumerate(coordinates):
-        if np.isnan(x) or np.isnan(y): continue
+    for i, (x, y) in enumerate(coordinates):
+        if np.isnan(x) or np.isnan(y):
+            continue
         pos = (int(x), int(y))
-        canvas = cv2.circle(canvas, pos, node_size, colors[i], -1, lineType=cv2.LINE_AA)
+        canvas = cv2.circle(
+            canvas, pos, node_size, colors[i], -1, lineType=cv2.LINE_AA
+        )
 
-    if opacity<1.0:
-        image = cv2.addWeighted(image, 1-opacity, canvas, opacity, 0)
+    if opacity < 1.0:
+        image = cv2.addWeighted(image, 1 - opacity, canvas, opacity, 0)
     return image
 
 
 def overlay_trajectory_on_video(
-        frames, trajectory, smoothing_kernel=1, highlight=None, 
-        min_opacity=0.2, max_opacity=1, num_ghosts=5, interval=2, 
-        plot_options={}):
-    
+    frames,
+    trajectory,
+    smoothing_kernel=1,
+    highlight=None,
+    min_opacity=0.2,
+    max_opacity=1,
+    num_ghosts=5,
+    interval=2,
+    plot_options={},
+    edges=[],
+):
     """
     Overlay a trajectory of keypoints on a video.
     """
     if smoothing_kernel > 0:
         trajectory = gaussian_filter1d(trajectory, smoothing_kernel, axis=0)
-        
-    opacities = np.repeat(np.linspace(max_opacity, min_opacity, num_ghosts+1), interval)  
-    for i in np.arange(0,trajectory.shape[0],interval):
-        for j,opacity in enumerate(opacities):
-            if i+j < frames.shape[0]:
-                plot_options['opacity'] = opacity
+
+    opacities = np.repeat(
+        np.linspace(max_opacity, min_opacity, num_ghosts + 1), interval
+    )
+    for i in np.arange(0, trajectory.shape[0], interval):
+        for j, opacity in enumerate(opacities):
+            if i + j < frames.shape[0]:
+                plot_options["opacity"] = opacity
                 if highlight is not None:
-                    start,end,highlight_factor = highlight
-                    if i+j < start or i+j > end:
-                        plot_options['opacity'] *= highlight_factor
-                frames[i+j] = overlay_keypoints_on_image(
-                    frames[i+j], trajectory[i], **plot_options)
+                    start, end, highlight_factor = highlight
+                    if i + j < start or i + j > end:
+                        plot_options["opacity"] *= highlight_factor
+                frames[i + j] = overlay_keypoints_on_image(
+                    frames[i + j], trajectory[i], edges=edges, **plot_options
+                )
     return frames
 
+
 def overlay_keypoints_on_video(
-    video_path, coordinates, skeleton=[], bodyparts=None, use_bodyparts=None, 
-    output_path=None, show_frame_numbers=True, text_color=(255,255,255), 
-    crop_size=None, frames=None, quality=7, centroid_smoothing_filter=10, 
-    plot_options={}):
-    """
-    Overlay keypoints on a video.
+    video_path,
+    coordinates,
+    skeleton=[],
+    bodyparts=None,
+    use_bodyparts=None,
+    output_path=None,
+    show_frame_numbers=True,
+    text_color=(255, 255, 255),
+    crop_size=None,
+    frames=None,
+    quality=7,
+    centroid_smoothing_filter=10,
+    plot_options={},
+):
+    """Overlay keypoints on a video.
 
     Parameters
     ----------
     video_path: str
         Path to a video file.
 
     coordinates: ndarray of shape (num_frames, num_keypoints, 2)
@@ -1479,324 +1839,474 @@
         Whether to overlay the frame number in the video.
 
     text_color: tuple of int, default=(255,255,255)
         Color for the frame number overlay.
 
     crop_size: int, default=None
         Size of the crop around the keypoints to overlay on the video.
-        If None, the entire video is used. 
+        If None, the entire video is used.
 
     frames: iterable of int, default=None
         Frames to overlay keypoints on. If None, all frames are used.
 
     quality: int, default=7
         Quality of the output video.
 
     centroid_smoothing_filter: int, default=10
         Amount of smoothing to determine cropping centroid.
 
     plot_options: dict, default={}
         Additional keyword arguments to pass to
         :py:func:`keypoint_moseq.viz.overlay_keypoints`.
     """
-    if output_path is None: 
-        output_path = os.path.splitext(video_path)[0] + '_keypoints.mp4'
+    if output_path is None:
+        output_path = os.path.splitext(video_path)[0] + "_keypoints.mp4"
 
     if bodyparts is not None:
         if use_bodyparts is not None:
-            coordinates = reindex_by_bodyparts(coordinates, bodyparts, use_bodyparts)
-        else: use_bodyparts = bodyparts
+            coordinates = reindex_by_bodyparts(
+                coordinates, bodyparts, use_bodyparts
+            )
+        else:
+            use_bodyparts = bodyparts
         edges = get_edges(use_bodyparts, skeleton)
-    else: edges = skeleton
+    else:
+        edges = skeleton
 
     if crop_size is not None:
         outliers = np.any(np.isnan(coordinates), axis=2)
         interpolated_coordinates = interpolate_keypoints(coordinates, outliers)
         crop_centroid = np.nanmedian(interpolated_coordinates, axis=1)
-        crop_centroid = gaussian_filter1d(crop_centroid, centroid_smoothing_filter, axis=0)
+        crop_centroid = gaussian_filter1d(
+            crop_centroid, centroid_smoothing_filter, axis=0
+        )
 
     with imageio.get_reader(video_path) as reader:
-        fps = reader.get_meta_data()['fps']
-        if frames is None: frames = np.arange(reader.count_frames())
+        fps = reader.get_meta_data()["fps"]
+        if frames is None:
+            frames = np.arange(reader.count_frames())
 
         with imageio.get_writer(
-            output_path, pixelformat='yuv420p', 
-            fps=fps, quality=quality) as writer:
-
-            for frame in tqdm.tqdm(frames):
+            output_path, pixelformat="yuv420p", fps=fps, quality=quality
+        ) as writer:
+            for frame in tqdm.tqdm(frames, ncols=72):
                 image = reader.get_data(frame)
 
                 image = overlay_keypoints_on_image(
-                    image, coordinates[frame], edges=edges, **plot_options)
+                    image, coordinates[frame], edges=edges, **plot_options
+                )
 
                 if crop_size is not None:
                     image = crop_image(image, crop_centroid[frame], crop_size)
 
                 if show_frame_numbers:
                     image = cv2.putText(
-                        image, f'Frame {frame}', (10, 20), cv2.FONT_HERSHEY_SIMPLEX, 
-                        0.5, text_color, 1, cv2.LINE_AA)
+                        image,
+                        f"Frame {frame}",
+                        (10, 20),
+                        cv2.FONT_HERSHEY_SIMPLEX,
+                        0.5,
+                        text_color,
+                        1,
+                        cv2.LINE_AA,
+                    )
 
                 writer.append_data(image)
 
 
+def matplotlib_colormap_to_plotly(cmap):
+    """
+    Convert a matplotlib colormap to a plotly colormap.
 
+    Parameters
+    ----------
+    cmap: str
+        Name of a matplotlib colormap.
 
-
-def crowd_movie(
-    instances, coordinates, centroids, lims, pre=30, post=60,
-    edges=[], plot_options={}):
-    """
-    Generate a crowd movie.
-
-    Crowd movies show many instances of a syllable by animating
-    their keypoint trajectories in a common coordinate system.
-    The trajectories are synchronized to syllable onset. The opacity 
-    of each instance increases at syllable onset and decreases at
-    syllable offset.
+    Returns
+    -------
+    pl_colorscale: list
+        Plotly colormap.
+    """
+    cmap = plt.colormaps[cmap]
+    pl_entries = 255
+    h = 1.0 / (pl_entries - 1)
+    pl_colorscale = []
+    for k in range(pl_entries):
+        C = (np.array(cmap(k * h)[:3]) * 255).astype(np.uint8)
+        pl_colorscale.append([k * h, "rgb" + str((C[0], C[1], C[2]))])
+    return pl_colorscale
+
+
+def add_3D_pose_to_plotly_fig(
+    fig,
+    coords,
+    edges,
+    keypoint_colormap="autumn",
+    node_size=6.0,
+    linewidth=3.0,
+    visible=True,
+    opacity=1,
+):
+    """
+    Add a 3D pose to a plotly figure.
 
     Parameters
     ----------
-    instances: list of tuples `(key, start, end)`
-        List of syllable instances to include in the grid movie,
-        where each instance is specified as a tuple with the session
-        name, start frame and end frame. 
-    
-    coordinates: dict of ndarrays of shape (num_frames, num_keypoints, dim)
-        Dictionary of keypoint coordinates, where each key is a session name.
-        
-    centroids: dict of ndarrays of shape (num_frames, dim)
-        Dictionary of animal centroids, where each key is a session name.
+    fig: plotly figure
+        Figure to which the pose should be added.
 
-    lims: array of shape (2, dim)
-        Axis limits for plotting keypoints in the crowd movies. 
+    coords: ndarray (N,3)
+        3D coordinates of the pose.
 
-    pre: int, default=30
-        Number of frames before syllable onset to include in the movie
+    edges: list of index pairs
+        Skeleton edges
 
-    post: int, default=60
-        Number of frames after syllable onset to include in the movie
+    keypoint_colormap: str, default='autumn'
+        Colormap to use for coloring keypoints.
 
-    plot_options: dict, default={}
-        Dictionary of options for rendering keypoints in the crowd
-        movies (see :py:func:`keypoint_moseq.util.overlay_keypoints_on_image`).
+    node_size: float, default=6.0
+        Size of keypoints.
 
-    Returns
-    -------
-    frames: array of shape `(post+pre, height, width, 3)`
-        Array of frames in the grid movie. `width` and 
-        `height` are determined by `lims`.
-    """
-    dim = coordinates[instances[0][0]].shape[2]
-    if dim == 3: warnings.warn(fill(
-        'Crowd movies are only supported for 2D keypoints. '
-        'Only the X and Y coordinates will be used.'))
+    linewidth: float, default=3.0
+        Width of skeleton edges.
 
-    h, w = (lims[1]-lims[0]).astype(int)
-    frames = np.zeros((post+pre, w, h, 3), dtype=np.uint8)
+    visibility: bool, default=True
+        Initial visibility state of the nodes and edges
+
+    opacity: float, default=1
+        Opacity of the nodes and edges (0-1)
+    """
+    marker = {
+        "size": node_size,
+        "color": np.linspace(0, 1, len(coords)),
+        "colorscale": matplotlib_colormap_to_plotly(keypoint_colormap),
+        "line": dict(color="black", width=0.5),
+        "opacity": opacity,
+    }
+
+    line = {"width": linewidth, "color": f"rgba(0,0,0,{opacity})"}
+
+    fig.add_trace(
+        plotly.graph_objs.Scatter3d(
+            x=coords[:, 0],
+            y=coords[:, 1],
+            z=coords[:, 2],
+            mode="markers",
+            visible=visible,
+            marker=marker,
+        )
+    )
+
+    for e in edges:
+        fig.add_trace(
+            plotly.graph_objs.Scatter3d(
+                x=coords[e, 0],
+                y=coords[e, 1],
+                z=coords[e, 2],
+                mode="lines",
+                visible=visible,
+                line=line,
+            )
+        )
+
+
+def plot_pcs_3D(
+    ymean,
+    ypcs,
+    edges,
+    keypoint_colormap,
+    savefig,
+    project_dir=None,
+    node_size=6,
+    linewidth=2,
+    height=400,
+    mean_pose_opacity=0.2,
+):
+    """
+    Visualize the components of a fitted PCA model based on 3D components.
 
-    for key, start, end in instances:
-        xy = coordinates[key][start-pre:start+post,:,:2]
-        xy = np.clip(xy, *lims[:,:2]) - lims[0,:2]
-        frames = overlay_trajectory_on_video(
-            frames, xy, plot_options=plot_options)
-
-        dot_radius=5
-        dot_color=(255,255,255)
-        cen = centroids[key][start-pre:start+post,:2]
-        cen = gaussian_filter1d(cen,1,axis=0)
-        cen = np.clip(cen, *lims[:,:2]) - lims[0,:2]
-        for i in range(pre, min(end-start+pre,pre+post)):
-            pos = (int(cen[i,0]),int(cen[i,1]))
-            frames[i] = cv2.circle(frames[i], pos, dot_radius, dot_color, -1, cv2.LINE_AA)
+    For each PC, a subplot shows the mean pose (semi-transparent) along
+    with a perturbation of the mean pose in the direction of the PC.
 
-    return frames
+    Parameters
+    ----------
+    ymean : ndarray (num_bodyparts, 3)
+        Mean pose.
 
+    ypcs : ndarray (num_pcs, num_bodyparts, 3)
+        Perturbations of the mean pose in the direction of each PC.
 
-def generate_crowd_movies(
-    coordinates, results=None, output_dir=None, name=None, 
-    project_dir=None, results_path=None, pre=30, post=60,
-    min_frequency=0.005, min_duration=3, num_instances=15,
-    use_reindexed=True, use_estimated_coords=False, skeleton=[], 
-    bodyparts=None, use_bodyparts=None, keypoint_colormap='autumn', 
-    fps=30, limits=None, plot_options={}, sampling_options={}, 
-    quality=7, **kwargs):
-    """
-    Generate crowd movies for a modeled dataset.
-
-    Crowd movies show many instances of a syllable and are useful in
-    figuring out what behavior the syllable captures 
-    (see :py:func:`keypoint_moseq.viz.crowd_movie`). This method
-    generates a crowd movie for each syllable that is used sufficiently
-    often (i.e. has at least `num_instances` instances with duration
-    of at least `min_duration` and an overall frequency of at least
-    `min_frequency`). The crowd movies are saved to `output_dir` if 
-    specified, or else to `{project_dir}/{name}/crowd_movies`.
+    edges : list of index pairs
+        Skeleton edges.
 
-    Parameters
-    ----------
-    coordinates: dict, default=None
-        Dictionary mapping session names to keypoint coordinates as 
-        ndarrays of shape (n_frames, n_bodyparts, 2). Required if
-        `use_estimated_coords=False`.
+    keypoint_colormap : str
+        Name of a matplotlib colormap to use for coloring the keypoints.
 
-    results: dict, default=None
-        Dictionary containing modeling results for a dataset (see
-        :py:func:`keypoint_moseq.fitting.apply_model`). Must have
-        the format::
+    savefig : bool
+        Whether to save the figure to a file. If true, the figure is
+        saved to `{project_dir}/pcs.html`
 
-            {
-                session_name1: {
-                    'syllables':              array of shape (n_frames,),
-                    'estimated_coordinates' : array of shape (n_frames, n_bodyparts, dim)
-                    'syllables_reindexed':    array of shape (n_frames,),
-                    'centroid':               array of shape (n_frames, dim),
-                    'heading' :               array of shape (n_frames,), 
-                },
-                ...  
-            }
-            
-        - `syllables` is required if `use_reindexed=False`
-        - `syllables_reindexed` is required if `use_reindexed=True`
-        - `centroid` is required if the sampling mode is 'density'
-        - `heading` is required if the sampling mode is 'density'
-        - `estimated_coordinates` is required if `use_estimated_coords=True`
-        
+    project_dir : str, default=None
+        Path to the project directory. Required if `savefig` is True.
 
-        If `results=None`, results will be loaded using either 
-        `results_path` or  `project_dir` and `name`.
+    node_size : float, default=30.0
+        Size of the keypoints in the figure.
 
-    output_dir: str, default=None
-        Directory where crowd movies should be saved. If None, 
-        movies will be saved to `{project_dir}/{name}/crowd_movies`.
+    linewidth: float, default=2.0
+        Width of edges in skeleton
 
-    name: str, default=None
-        Name of the model. Required to load results if `results` is 
-        None and `results_path` is None. Required to save crowd
-        movies if `output_dir` is None.
+    height : int, default=400
+        Height of the figure in pixels.
 
-    project_dir: str, default=None
-        Project directory. Required to load results if `results` is 
-        None and `results_path` is None. Required to save crowd
-        movies if `output_dir` is None.
+    mean_pose_opacity: float, default=0.4
+        Opacity of the mean pose
+    """
+    from plotly.subplots import make_subplots
 
-    results_path: str, default=None
-        Path to a results file. If None, results will be loaded from
-        `{project_dir}/{name}/results.h5`.
+    fig = make_subplots(rows=1, cols=1, specs=[[{"type": "scatter3d"}]])
+
+    def visibility_mask(i):
+        visible = np.zeros((len(edges) + 1) * (len(ypcs) + 1))
+        visible[-(len(edges) + 1) :] = 1
+        visible[(len(edges) + 1) * i : (len(edges) + 1) * (i + 1)] = 1
+        return visible > 0
+
+    steps = []
+    for i, coords in enumerate(ypcs):
+        add_3D_pose_to_plotly_fig(
+            fig,
+            coords,
+            edges,
+            visible=(i == 0),
+            node_size=node_size,
+            linewidth=linewidth,
+            keypoint_colormap=keypoint_colormap,
+        )
+
+        steps.append(
+            dict(
+                method="update",
+                label=f"PC {i+1}",
+                args=[{"visible": visibility_mask(i)}],
+            )
+        )
+
+    add_3D_pose_to_plotly_fig(
+        fig,
+        ymean,
+        edges,
+        opacity=mean_pose_opacity,
+        node_size=node_size,
+        linewidth=linewidth,
+        keypoint_colormap=keypoint_colormap,
+    )
+
+    fig.update_layout(
+        height=height,
+        showlegend=False,
+        sliders=[dict(steps=steps)],
+        scene=dict(
+            xaxis=dict(showgrid=False, showbackground=False),
+            yaxis=dict(showgrid=False, showbackground=False),
+            zaxis=dict(showgrid=False, showline=True, linecolor="black"),
+            bgcolor="white",
+            aspectmode="data",
+        ),
+        margin=dict(l=20, r=20, b=0, t=0, pad=10),
+    )
 
-    num_instances: int, default=15
-        Number of syllable instances per crowd movie.
+    if savefig:
+        assert project_dir is not None, fill(
+            "The `savefig` option requires a `project_dir`"
+        )
+        save_path = os.path.join(project_dir, f"pcs.html")
+        fig.write_html(save_path)
+        print(f"Saved interactive plot to {save_path}")
+
+    fig.show()
+
+
+def plot_trajectories_3D(
+    Xs,
+    titles,
+    edges,
+    output_dir,
+    keypoint_colormap="autumn",
+    node_size=8,
+    linewidth=3,
+    height=500,
+    skiprate=1,
+):
+    """
+    Visualize a set of 3D trajectories.
 
-    min_frequency: float, default=0.005
-        Minimum frequency of a syllable to be included in the crowd movies.
+    Parameters
+    ----------
+    Xs : list of ndarrays (num_syllables, num_frames, num_bodyparts, 3)
+        Trajectories to visualize.
 
-    min_duration: int, default=3
-        Minimum duration of a syllable instance to be included in the 
-        crowd movie for that syllable. 
+    titles : list of str
+        Title for each trajectory.
 
-    use_reindexed: bool, default=True
-        Whether to use label syllables by their frequency rank (True) or
-        or their original label (False). When reindexing, "0"  represents
-        the most frequent syllable).
+    edges : list of index pairs
+        Skeleton edges.
 
-    bodyparts: list of str, default=None
-        List of bodypart names in `coordinates`. 
+    output_dir : str
+        Path to save the interactive plot.
 
-    use_bodyparts: list of str, default=None
-        Ordered list of bodyparts to include in the crowd
-        movies. If None, all bodyparts will be included.
-        
-    skeleton: list, default=[]
-        List of edges that define the skeleton, where each edge is a
-        pair of bodypart names or a pair of indexes.
-        
-    keypoint_colormap: str, default='autumn'
+    keypoint_colormap : str, default='autumn'
         Name of a matplotlib colormap to use for coloring the keypoints.
-        
-    fps: int, default=30
-        Frames per second of the crowd movies.
 
-    limits: array, default=None
-        Axis limits for plotting keypoints in the crowd movies. If None,
-        limits will be inferred automatically from `coordinates`.
-        
-    plot_options: dict, default={}
-        Dictionary of options for rendering keypoints in the crowd
-        movies (see :py:func:`keypoint_moseq.util.overlay_keypoints_on_image`).
-        
-    sampling_options: dict, default={}
-        Dictionary of options for sampling syllable instances (see
-        :py:func:`keypoint_moseq.util.sample_instances`).
+    node_size : float, default=8.0
+        Size of the keypoints in the figure.
 
-    quality: int, default=7
-        Quality of the crowd movies. Higher values result in higher
-        quality movies but larger file sizes.
-    """    
-    if output_dir is None:
-        assert project_dir is not None and name is not None, fill(
-            'Either specify the `output_dir` where crowd movies should '
-            'be saved or include a `project_dir` and `name`')
-        output_dir = os.path.join(project_dir,name, 'crowd_movies')
-    if not os.path.exists(output_dir): os.makedirs(output_dir)
-    print(f'Writing crowd movies to {output_dir}')
-
-    if results is None: results = load_results(
-        name=name, project_dir=project_dir, path=results_path)
-        
-    if use_estimated_coords:
-        coordinates = {k:v['estimated_coordinates'] for k,v in results.items()}
-    elif bodyparts is not None and use_bodyparts is not None:
-        coordinates = reindex_by_bodyparts(coordinates, bodyparts, use_bodyparts)
-
-    syllable_key = 'syllables' + ('_reindexed' if use_reindexed else '')
-    syllables = {k:v[syllable_key] for k,v in results.items()}
-    plot_options.update({'keypoint_colormap':keypoint_colormap})
-
-    if limits is None: 
-        limits = get_limits(coordinates, blocksize=16)
-
-    k = list(results.keys())[0]
-    if 'heading' in results[k]:
-        headings = {k:v['heading'] for k,v in results.items()}
-    else: headings = None
-        
-    if 'centroid' in results[k]:
-        centroids = {k:v['centroid'] for k,v in results.items()}
-    else:
-        outliers = np.any(np.isnan(coordinates), axis=2)
-        interpolated_coordinates = interpolate_keypoints(coordinates, outliers)
-        centroids = {k:v.mean(1) for k,v in interpolated_coordinates.items()}
+    linewidth: float, default=3.0
+        Width of edges in skeleton
 
-    edges = []
-    if len(skeleton)>0: 
-        if isinstance(skeleton[0][0],str):
-            assert use_bodyparts is not None, fill(
-                'If skeleton edges are specified using bodypart names, '
-                '`use_bodyparts` must be specified')
-            edges = get_edges(use_bodyparts, skeleton)
-        else: edges = skeleton
+    height : int, default=500
+        Height of the figure in pixels.
 
-    syllable_instances = get_syllable_instances(
-        syllables, pre=pre, post=post, min_duration=min_duration,
-        min_frequency=min_frequency, min_instances=num_instances)
-    
-    if len(syllable_instances) == 0:
-        warnings.warn(fill(
-            'No syllables with sufficient instances to make a crowd movie. '
-            'This usually occurs when all frames have the same syllable label '
-            '(use `plot_syllable_frequencies` to check if this is the case)'))
-        return
+    skiprate : int, default=1
+        Plot every `skiprate` frames.
+    """
+    from plotly.subplots import make_subplots
 
-    sampled_instances = sample_instances(
-        syllable_instances, num_instances, coordinates=coordinates, 
-        centroids=centroids, headings=headings, **sampling_options)
+    fig = make_subplots(rows=1, cols=1, specs=[[{"type": "scatter3d"}]])
+    Xs = Xs[:, ::skiprate]
+
+    def visibility_mask(i):
+        n = (len(edges) + 1) * len(Xs[1])
+        visible = np.zeros(n * len(Xs))
+        visible[n * i : n * (i + 1)] = 1
+        return visible > 0
+
+    steps = []
+    for i, X in enumerate(Xs):
+        opacities = np.linspace(0.3, 1, len(X) + 1)[1:] ** 2
+        for coords, opacity in zip(X, opacities):
+            add_3D_pose_to_plotly_fig(
+                fig,
+                coords,
+                edges,
+                visible=(i == 0),
+                node_size=node_size,
+                linewidth=linewidth,
+                keypoint_colormap=keypoint_colormap,
+                opacity=opacity,
+            )
+
+        steps.append(
+            dict(
+                method="update",
+                label=titles[i],
+                args=[{"visible": visibility_mask(i)}],
+            )
+        )
+
+    fig.update_layout(
+        height=height,
+        showlegend=False,
+        sliders=[dict(steps=steps)],
+        scene=dict(
+            xaxis=dict(showgrid=False, showbackground=False),
+            yaxis=dict(showgrid=False, showbackground=False),
+            zaxis=dict(showgrid=False, showline=True, linecolor="black"),
+            bgcolor="white",
+            aspectmode="data",
+        ),
+        margin=dict(l=20, r=20, b=0, t=0, pad=10),
+    )
+
+    if output_dir is not None:
+        save_path = os.path.join(output_dir, f"all_trajectories.html")
+        fig.write_html(save_path)
+        print(f"Saved interactive trajectories plot to {save_path}")
+
+    fig.show()
+
+
+def plot_similarity_dendrogram(
+    coordinates,
+    results,
+    project_dir=None,
+    model_name=None,
+    save_path=None,
+    metric="cosine",
+    pre=5,
+    post=15,
+    min_frequency=0.005,
+    min_duration=3,
+    bodyparts=None,
+    use_bodyparts=None,
+    density_sample=False,
+    sampling_options={},
+    figsize=(6, 3),
+    **kwargs,
+):
+    """Plot a dendrogram showing the similarity between syllable trajectories.
+
+    The dendrogram is saved to `{save_path}` if it is provided, or
+    else to `{project_dir}/{model_name}/similarity_dendrogram.pdf`. Plot-
+    related parameters are described below. For the remaining parameters
+    see (:py:func:`keypoint_moseq.util.get_typical_trajectories`)
 
-    for syllable,instances in tqdm.tqdm(
-        sampled_instances.items(), desc='Generating crowd movies'):
-        
-        frames = crowd_movie(
-            instances, coordinates, centroids, pre=pre, post=post,
-            edges=edges, lims=limits, plot_options=plot_options)
+    Parameters
+    ----------
+    coordinates: dict
+        Dictionary mapping recording names to keypoint coordinates as
+        ndarrays of shape (n_frames, n_bodyparts, [2 or 3]).
 
-        path = os.path.join(output_dir, f'syllable{syllable}.mp4')
-        write_video_clip(frames, path, fps=fps, quality=quality)
-            
+    results: dict
+        Dictionary containing modeling results for a dataset (see
+        :py:func:`keypoint_moseq.fitting.extract_results`).
+
+    project_dir: str, default=None
+        Project directory. Required to save figure if `save_path` is None.
+
+    model_name: str, default=None
+        Model name. Required to save figure if `save_path` is None.
+
+    save_path: str, default=None
+        Path to save the dendrogram plot (do not include an extension).
+        If None, the plot will be saved  to
+        `{project_dir}/{name}/similarity_dendrogram.[pdf/png]`.
+
+    metric: str, default='cosine'
+        Distance metric to use. See :py:func:`scipy.spatial.pdist` for options.
+
+    figsize: tuple of float, default=(10,5)
+        Size of the dendrogram plot.
+    """
+    save_path = _get_path(
+        project_dir, model_name, save_path, "similarity_dendrogram"
+    )
+
+    distances, syllable_ixs = syllable_similarity(
+        coordinates,
+        results,
+        metric,
+        pre,
+        post,
+        min_frequency,
+        min_duration,
+        bodyparts,
+        use_bodyparts,
+        density_sample,
+        sampling_options,
+    )
+
+    Z = linkage(squareform(distances), "complete")
+
+    fig, ax = plt.subplots(1, 1)
+    labels = [f"Syllable {s}" for s in syllable_ixs]
+    dendrogram(Z, labels=labels, leaf_font_size=10, ax=ax, leaf_rotation=90)
+
+    ax.set_yticks([])
+    for spine in ax.spines.values():
+        spine.set_color("lightgray")
+    ax.set_title("Syllable similarity")
+    fig.set_size_inches(figsize)
+
+    print(f"Saving dendrogram plot to {save_path}")
+    for ext in ["pdf", "png"]:
+        plt.savefig(save_path + "." + ext)
```

### Comparing `keypoint-moseq-0.1.5/setup.cfg` & `keypoint-moseq-0.2.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -21,17 +21,26 @@
 	statsmodels
 	pyyaml
 	vidio
 	holoviews[recommended]
 	bokeh
 	pandas
 	tables
+	networkx
+	sleap_io
+	pynwb
+	ndx_pose
+	plotly
+	jupyter_nbextensions_configurator
+	jupyter_bokeh==2.0.3
+	qgrid==1.3.1
+	ipywidgets==7.5.1
 	tabulate
 	jaxtyping==0.2.14
-	jax-moseq==0.0.3
+	jax-moseq==0.0.5
 
 [options.package_data]
 * = *.md
 
 [versioneer]
 VCS = git
 style = pep440
```

### Comparing `keypoint-moseq-0.1.5/versioneer.py` & `keypoint-moseq-0.2.0/versioneer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-
 # Version: 0.28
-
 """The Versioneer - like a rocketeer, but for versions.
 
 The Versioneer
 ==============
 
 * like a rocketeer, but for versions!
 * https://github.com/python-versioneer/python-versioneer
@@ -344,33 +342,37 @@
     versioneer_py = os.path.join(root, "versioneer.py")
     if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
         # allow 'python path/to/setup.py COMMAND'
         root = os.path.dirname(os.path.realpath(os.path.abspath(sys.argv[0])))
         setup_py = os.path.join(root, "setup.py")
         versioneer_py = os.path.join(root, "versioneer.py")
     if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
-        err = ("Versioneer was unable to run the project root directory. "
-               "Versioneer requires setup.py to be executed from "
-               "its immediate directory (like 'python setup.py COMMAND'), "
-               "or in a way that lets it use sys.argv[0] to find the root "
-               "(like 'python path/to/setup.py COMMAND').")
+        err = (
+            "Versioneer was unable to run the project root directory. "
+            "Versioneer requires setup.py to be executed from "
+            "its immediate directory (like 'python setup.py COMMAND'), "
+            "or in a way that lets it use sys.argv[0] to find the root "
+            "(like 'python path/to/setup.py COMMAND')."
+        )
         raise VersioneerBadRootError(err)
     try:
         # Certain runtime workflows (setup.py install/develop in a setuptools
         # tree) execute all dependencies in a single python process, so
         # "versioneer" may be imported multiple times, and python's shared
         # module-import table will cache the first one. So we can't use
         # os.path.dirname(__file__), as that will find whichever
         # versioneer.py was first imported, even in later projects.
         my_path = os.path.realpath(os.path.abspath(__file__))
         me_dir = os.path.normcase(os.path.splitext(my_path)[0])
         vsr_dir = os.path.normcase(os.path.splitext(versioneer_py)[0])
         if me_dir != vsr_dir and "VERSIONEER_PEP518" not in globals():
-            print("Warning: build in %s is using versioneer.py from %s"
-                  % (os.path.dirname(my_path), versioneer_py))
+            print(
+                "Warning: build in %s is using versioneer.py from %s"
+                % (os.path.dirname(my_path), versioneer_py)
+            )
     except NameError:
         pass
     return root
 
 
 def get_config_from_root(root):
     """Read the project setup.cfg file to determine Versioneer config."""
@@ -380,29 +382,29 @@
     # the top of versioneer.py for instructions on writing your setup.cfg .
     root = Path(root)
     pyproject_toml = root / "pyproject.toml"
     setup_cfg = root / "setup.cfg"
     section = None
     if pyproject_toml.exists() and have_tomllib:
         try:
-            with open(pyproject_toml, 'rb') as fobj:
+            with open(pyproject_toml, "rb") as fobj:
                 pp = tomllib.load(fobj)
-            section = pp['tool']['versioneer']
+            section = pp["tool"]["versioneer"]
         except (tomllib.TOMLDecodeError, KeyError):
             pass
     if not section:
         parser = configparser.ConfigParser()
         with open(setup_cfg) as cfg_file:
             parser.read_file(cfg_file)
         parser.get("versioneer", "VCS")  # raise error if missing
 
         section = parser["versioneer"]
 
     cfg = VersioneerConfig()
-    cfg.VCS = section['VCS']
+    cfg.VCS = section["VCS"]
     cfg.style = section.get("style", "")
     cfg.versionfile_source = section.get("versionfile_source")
     cfg.versionfile_build = section.get("versionfile_build")
     cfg.tag_prefix = section.get("tag_prefix")
     if cfg.tag_prefix in ("''", '""', None):
         cfg.tag_prefix = ""
     cfg.parentdir_prefix = section.get("parentdir_prefix")
@@ -417,23 +419,26 @@
 # these dictionaries contain VCS-specific tools
 LONG_VERSION_PY: Dict[str, str] = {}
 HANDLERS: Dict[str, Dict[str, Callable]] = {}
 
 
 def register_vcs_handler(vcs, method):  # decorator
     """Create decorator to mark a method as the handler of a VCS."""
+
     def decorate(f):
         """Store f in HANDLERS[vcs][method]."""
         HANDLERS.setdefault(vcs, {})[method] = f
         return f
+
     return decorate
 
 
-def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False,
-                env=None):
+def run_command(
+    commands, args, cwd=None, verbose=False, hide_stderr=False, env=None
+):
     """Call the given command(s)."""
     assert isinstance(commands, list)
     process = None
 
     popen_kwargs = {}
     if sys.platform == "win32":
         # This hides the console window if pythonw.exe is used
@@ -441,18 +446,22 @@
         startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
         popen_kwargs["startupinfo"] = startupinfo
 
     for command in commands:
         try:
             dispcmd = str([command] + args)
             # remember shell=False, so use git.cmd on windows, not just git
-            process = subprocess.Popen([command] + args, cwd=cwd, env=env,
-                                       stdout=subprocess.PIPE,
-                                       stderr=(subprocess.PIPE if hide_stderr
-                                               else None), **popen_kwargs)
+            process = subprocess.Popen(
+                [command] + args,
+                cwd=cwd,
+                env=env,
+                stdout=subprocess.PIPE,
+                stderr=(subprocess.PIPE if hide_stderr else None),
+                **popen_kwargs,
+            )
             break
         except OSError:
             e = sys.exc_info()[1]
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %s" % dispcmd)
@@ -467,15 +476,17 @@
         if verbose:
             print("unable to run %s (error)" % dispcmd)
             print("stdout was %s" % stdout)
         return None, process.returncode
     return stdout, process.returncode
 
 
-LONG_VERSION_PY['git'] = r'''
+LONG_VERSION_PY[
+    "git"
+] = r'''
 # This file helps to compute a version number in source trees obtained from
 # git-archive tarball (such as those provided by githubs download-from-tag
 # feature). Distribution tarballs (built by setup.py sdist) and build
 # directories (produced by setup.py build) will contain a much shorter file
 # that just contains the computed version number.
 
 # This file is released into the public domain.
@@ -1183,49 +1194,56 @@
         if verbose:
             print("keywords are unexpanded, not using")
         raise NotThisMethod("unexpanded keywords, not a git-archive tarball")
     refs = {r.strip() for r in refnames.strip("()").split(",")}
     # starting in git-1.8.3, tags are listed as "tag: foo-1.0" instead of
     # just "foo-1.0". If we see a "tag: " prefix, prefer those.
     TAG = "tag: "
-    tags = {r[len(TAG):] for r in refs if r.startswith(TAG)}
+    tags = {r[len(TAG) :] for r in refs if r.startswith(TAG)}
     if not tags:
         # Either we're using git < 1.8.3, or there really are no tags. We use
         # a heuristic: assume all version tags have a digit. The old git %d
         # expansion behaves like git log --decorate=short and strips out the
         # refs/heads/ and refs/tags/ prefixes that would let us distinguish
         # between branches and tags. By ignoring refnames without digits, we
         # filter out many common branch names like "release" and
         # "stabilization", as well as "HEAD" and "master".
-        tags = {r for r in refs if re.search(r'\d', r)}
+        tags = {r for r in refs if re.search(r"\d", r)}
         if verbose:
             print("discarding '%s', no digits" % ",".join(refs - tags))
     if verbose:
         print("likely tags: %s" % ",".join(sorted(tags)))
     for ref in sorted(tags):
         # sorting will prefer e.g. "2.0" over "2.0rc1"
         if ref.startswith(tag_prefix):
-            r = ref[len(tag_prefix):]
+            r = ref[len(tag_prefix) :]
             # Filter out refs that exactly match prefix or that don't start
             # with a number once the prefix is stripped (mostly a concern
             # when prefix is '')
-            if not re.match(r'\d', r):
+            if not re.match(r"\d", r):
                 continue
             if verbose:
                 print("picking %s" % r)
-            return {"version": r,
-                    "full-revisionid": keywords["full"].strip(),
-                    "dirty": False, "error": None,
-                    "date": date}
+            return {
+                "version": r,
+                "full-revisionid": keywords["full"].strip(),
+                "dirty": False,
+                "error": None,
+                "date": date,
+            }
     # no suitable tags, so version is "0+unknown", but full hex is still there
     if verbose:
         print("no suitable tags, using unknown + full revision id")
-    return {"version": "0+unknown",
-            "full-revisionid": keywords["full"].strip(),
-            "dirty": False, "error": "no suitable tags", "date": None}
+    return {
+        "version": "0+unknown",
+        "full-revisionid": keywords["full"].strip(),
+        "dirty": False,
+        "error": "no suitable tags",
+        "date": None,
+    }
 
 
 @register_vcs_handler("git", "pieces_from_vcs")
 def git_pieces_from_vcs(tag_prefix, root, verbose, runner=run_command):
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
@@ -1239,43 +1257,54 @@
     # GIT_DIR can interfere with correct operation of Versioneer.
     # It may be intended to be passed to the Versioneer-versioned project,
     # but that should not change where we get our version from.
     env = os.environ.copy()
     env.pop("GIT_DIR", None)
     runner = functools.partial(runner, env=env)
 
-    _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root,
-                   hide_stderr=not verbose)
+    _, rc = runner(
+        GITS, ["rev-parse", "--git-dir"], cwd=root, hide_stderr=not verbose
+    )
     if rc != 0:
         if verbose:
             print("Directory %s not under git control" % root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = runner(GITS, [
-        "describe", "--tags", "--dirty", "--always", "--long",
-        "--match", f"{tag_prefix}[[:digit:]]*"
-    ], cwd=root)
+    describe_out, rc = runner(
+        GITS,
+        [
+            "describe",
+            "--tags",
+            "--dirty",
+            "--always",
+            "--long",
+            "--match",
+            f"{tag_prefix}[[:digit:]]*",
+        ],
+        cwd=root,
+    )
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
     full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
     full_out = full_out.strip()
 
     pieces = {}
     pieces["long"] = full_out
     pieces["short"] = full_out[:7]  # maybe improved later
     pieces["error"] = None
 
-    branch_name, rc = runner(GITS, ["rev-parse", "--abbrev-ref", "HEAD"],
-                             cwd=root)
+    branch_name, rc = runner(
+        GITS, ["rev-parse", "--abbrev-ref", "HEAD"], cwd=root
+    )
     # --abbrev-ref was added in git-1.6.3
     if rc != 0 or branch_name is None:
         raise NotThisMethod("'git rev-parse --abbrev-ref' returned error")
     branch_name = branch_name.strip()
 
     if branch_name == "HEAD":
         # If we aren't exactly on a branch, pick a branch which represents
@@ -1307,65 +1336,70 @@
     # TAG might have hyphens.
     git_describe = describe_out
 
     # look for -dirty suffix
     dirty = git_describe.endswith("-dirty")
     pieces["dirty"] = dirty
     if dirty:
-        git_describe = git_describe[:git_describe.rindex("-dirty")]
+        git_describe = git_describe[: git_describe.rindex("-dirty")]
 
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
-        mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
+        mo = re.search(r"^(.+)-(\d+)-g([0-9a-f]+)$", git_describe)
         if not mo:
             # unparsable. Maybe git-describe is misbehaving?
-            pieces["error"] = ("unable to parse git-describe output: '%s'"
-                               % describe_out)
+            pieces["error"] = (
+                "unable to parse git-describe output: '%s'" % describe_out
+            )
             return pieces
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
             if verbose:
                 fmt = "tag '%s' doesn't start with prefix '%s'"
                 print(fmt % (full_tag, tag_prefix))
-            pieces["error"] = ("tag '%s' doesn't start with prefix '%s'"
-                               % (full_tag, tag_prefix))
+            pieces["error"] = "tag '%s' doesn't start with prefix '%s'" % (
+                full_tag,
+                tag_prefix,
+            )
             return pieces
-        pieces["closest-tag"] = full_tag[len(tag_prefix):]
+        pieces["closest-tag"] = full_tag[len(tag_prefix) :]
 
         # distance: number of commits since tag
         pieces["distance"] = int(mo.group(2))
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
         out, rc = runner(GITS, ["rev-list", "HEAD", "--left-right"], cwd=root)
         pieces["distance"] = len(out.split())  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
-    date = runner(GITS, ["show", "-s", "--format=%ci", "HEAD"], cwd=root)[0].strip()
+    date = runner(GITS, ["show", "-s", "--format=%ci", "HEAD"], cwd=root)[
+        0
+    ].strip()
     # Use only the last line.  Previous lines may contain GPG signature
     # information.
     date = date.splitlines()[-1]
     pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
 
     return pieces
 
 
 def do_vcs_install(versionfile_source, ipy):
     """Git-specific installation logic for Versioneer.
 
     For Git, this means creating/changing .gitattributes to mark _version.py
-    for export-subst keyword substitution.
+    for export- subst keyword substitution.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
     files = [versionfile_source]
     if ipy:
         files.append(ipy)
@@ -1403,23 +1437,29 @@
     two directory levels for an appropriately named parent directory
     """
     rootdirs = []
 
     for _ in range(3):
         dirname = os.path.basename(root)
         if dirname.startswith(parentdir_prefix):
-            return {"version": dirname[len(parentdir_prefix):],
-                    "full-revisionid": None,
-                    "dirty": False, "error": None, "date": None}
+            return {
+                "version": dirname[len(parentdir_prefix) :],
+                "full-revisionid": None,
+                "dirty": False,
+                "error": None,
+                "date": None,
+            }
         rootdirs.append(root)
         root = os.path.dirname(root)  # up a level
 
     if verbose:
-        print("Tried directories %s but none started with prefix %s" %
-              (str(rootdirs), parentdir_prefix))
+        print(
+            "Tried directories %s but none started with prefix %s"
+            % (str(rootdirs), parentdir_prefix)
+        )
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
 SHORT_VERSION_PY = """
 # This file was generated by 'versioneer.py' (0.28) from
 # revision-control system data, or from the parent directory name of an
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
@@ -1440,29 +1480,36 @@
 def versions_from_file(filename):
     """Try to determine the version from _version.py if present."""
     try:
         with open(filename) as f:
             contents = f.read()
     except OSError:
         raise NotThisMethod("unable to read _version.py")
-    mo = re.search(r"version_json = '''\n(.*)'''  # END VERSION_JSON",
-                   contents, re.M | re.S)
+    mo = re.search(
+        r"version_json = '''\n(.*)'''  # END VERSION_JSON",
+        contents,
+        re.M | re.S,
+    )
     if not mo:
-        mo = re.search(r"version_json = '''\r\n(.*)'''  # END VERSION_JSON",
-                       contents, re.M | re.S)
+        mo = re.search(
+            r"version_json = '''\r\n(.*)'''  # END VERSION_JSON",
+            contents,
+            re.M | re.S,
+        )
     if not mo:
         raise NotThisMethod("no version_json in _version.py")
     return json.loads(mo.group(1))
 
 
 def write_to_version_file(filename, versions):
     """Write the given version number to the given _version.py file."""
     os.unlink(filename)
-    contents = json.dumps(versions, sort_keys=True,
-                          indent=1, separators=(",", ": "))
+    contents = json.dumps(
+        versions, sort_keys=True, indent=1, separators=(",", ": ")
+    )
     with open(filename, "w") as f:
         f.write(SHORT_VERSION_PY % contents)
 
     print("set %s to '%s'" % (filename, versions["version"]))
 
 
 def plus_or_dot(pieces):
@@ -1486,16 +1533,15 @@
         if pieces["distance"] or pieces["dirty"]:
             rendered += plus_or_dot(pieces)
             rendered += "%d.g%s" % (pieces["distance"], pieces["short"])
             if pieces["dirty"]:
                 rendered += ".dirty"
     else:
         # exception #1
-        rendered = "0+untagged.%d.g%s" % (pieces["distance"],
-                                          pieces["short"])
+        rendered = "0+untagged.%d.g%s" % (pieces["distance"], pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
 def render_pep440_branch(pieces):
     """TAG[[.dev0]+DISTANCE.gHEX[.dirty]] .
@@ -1516,44 +1562,48 @@
             if pieces["dirty"]:
                 rendered += ".dirty"
     else:
         # exception #1
         rendered = "0"
         if pieces["branch"] != "master":
             rendered += ".dev0"
-        rendered += "+untagged.%d.g%s" % (pieces["distance"],
-                                          pieces["short"])
+        rendered += "+untagged.%d.g%s" % (pieces["distance"], pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
 def pep440_split_post(ver):
     """Split pep440 version string at the post-release segment.
 
-    Returns the release segments before the post-release and the
-    post-release version number (or -1 if no post-release segment is present).
+    Returns the release segments before the post-release and the post-release
+    version number (or -1 if no post-release segment is present).
     """
     vc = str.split(ver, ".post")
     return vc[0], int(vc[1] or 0) if len(vc) == 2 else None
 
 
 def render_pep440_pre(pieces):
     """TAG[.postN.devDISTANCE] -- No -dirty.
 
     Exceptions:
     1: no tags. 0.post0.devDISTANCE
     """
     if pieces["closest-tag"]:
         if pieces["distance"]:
             # update the post release segment
-            tag_version, post_version = pep440_split_post(pieces["closest-tag"])
+            tag_version, post_version = pep440_split_post(
+                pieces["closest-tag"]
+            )
             rendered = tag_version
             if post_version is not None:
-                rendered += ".post%d.dev%d" % (post_version + 1, pieces["distance"])
+                rendered += ".post%d.dev%d" % (
+                    post_version + 1,
+                    pieces["distance"],
+                )
             else:
                 rendered += ".post0.dev%d" % (pieces["distance"])
         else:
             # no commits, use the tag as the version
             rendered = pieces["closest-tag"]
     else:
         # exception #1
@@ -1678,19 +1728,21 @@
         rendered += "-dirty"
     return rendered
 
 
 def render(pieces, style):
     """Render the given version pieces into the requested style."""
     if pieces["error"]:
-        return {"version": "unknown",
-                "full-revisionid": pieces.get("long"),
-                "dirty": None,
-                "error": pieces["error"],
-                "date": None}
+        return {
+            "version": "unknown",
+            "full-revisionid": pieces.get("long"),
+            "dirty": None,
+            "error": pieces["error"],
+            "date": None,
+        }
 
     if not style or style == "default":
         style = "pep440"  # the default
 
     if style == "pep440":
         rendered = render_pep440(pieces)
     elif style == "pep440-branch":
@@ -1706,17 +1758,21 @@
     elif style == "git-describe":
         rendered = render_git_describe(pieces)
     elif style == "git-describe-long":
         rendered = render_git_describe_long(pieces)
     else:
         raise ValueError("unknown style '%s'" % style)
 
-    return {"version": rendered, "full-revisionid": pieces["long"],
-            "dirty": pieces["dirty"], "error": None,
-            "date": pieces.get("date")}
+    return {
+        "version": rendered,
+        "full-revisionid": pieces["long"],
+        "dirty": pieces["dirty"],
+        "error": None,
+        "date": pieces.get("date"),
+    }
 
 
 class VersioneerBadRootError(Exception):
     """The project root directory is unknown or missing key files."""
 
 
 def get_versions(verbose=False):
@@ -1731,16 +1787,17 @@
     root = get_root()
     cfg = get_config_from_root(root)
 
     assert cfg.VCS is not None, "please set [versioneer]VCS= in setup.cfg"
     handlers = HANDLERS.get(cfg.VCS)
     assert handlers, "unrecognized VCS '%s'" % cfg.VCS
     verbose = verbose or cfg.verbose
-    assert cfg.versionfile_source is not None, \
-        "please set versioneer.versionfile_source"
+    assert (
+        cfg.versionfile_source is not None
+    ), "please set versioneer.versionfile_source"
     assert cfg.tag_prefix is not None, "please set versioneer.tag_prefix"
 
     versionfile_abs = os.path.join(root, cfg.versionfile_source)
 
     # extract version from first of: _version.py, VCS command (e.g. 'git
     # describe'), parentdir. This is meant to work for developers using a
     # source checkout, for users of a tarball created by 'setup.py sdist',
@@ -1786,29 +1843,33 @@
             return ver
     except NotThisMethod:
         pass
 
     if verbose:
         print("unable to compute version")
 
-    return {"version": "0+unknown", "full-revisionid": None,
-            "dirty": None, "error": "unable to compute version",
-            "date": None}
+    return {
+        "version": "0+unknown",
+        "full-revisionid": None,
+        "dirty": None,
+        "error": "unable to compute version",
+        "date": None,
+    }
 
 
 def get_version():
     """Get the short version string for this project."""
     return get_versions()["version"]
 
 
 def get_cmdclass(cmdclass=None):
     """Get the custom setuptools subclasses used by Versioneer.
 
-    If the package uses a different cmdclass (e.g. one from numpy), it
-    should be provide as an argument.
+    If the package uses a different cmdclass (e.g. one from numpy), it should
+    be provide as an argument.
     """
     if "versioneer" in sys.modules:
         del sys.modules["versioneer"]
         # this fixes the "python setup.py develop" case (also 'install' and
         # 'easy_install .'), in which subdependencies of the main project are
         # built (using setup.py bdist_egg) in the same python process. Assume
         # a main project A and a dependency B, which use different versions
@@ -1841,14 +1902,15 @@
             vers = get_versions(verbose=True)
             print("Version: %s" % vers["version"])
             print(" full-revisionid: %s" % vers.get("full-revisionid"))
             print(" dirty: %s" % vers.get("dirty"))
             print(" date: %s" % vers.get("date"))
             if vers["error"]:
                 print(" error: %s" % vers["error"])
+
     cmds["version"] = cmd_version
 
     # we override "build_py" in setuptools
     #
     # most invocation pathways end up running build_py:
     #  distutils/build -> build_py
     #  distutils/install -> distutils/build ->..
@@ -1862,16 +1924,16 @@
     #   then does setup.py bdist_wheel, or sometimes setup.py install
     #  setup.py egg_info -> ?
 
     # pip install -e . and setuptool/editable_wheel will invoke build_py
     # but the build_py command is not expected to copy any files.
 
     # we override different "build_py" commands for both environments
-    if 'build_py' in cmds:
-        _build_py = cmds['build_py']
+    if "build_py" in cmds:
+        _build_py = cmds["build_py"]
     else:
         from setuptools.command.build_py import build_py as _build_py
 
     class cmd_build_py(_build_py):
         def run(self):
             root = get_root()
             cfg = get_config_from_root(root)
@@ -1880,22 +1942,24 @@
             if getattr(self, "editable_mode", False):
                 # During editable installs `.py` and data files are
                 # not copied to build_lib
                 return
             # now locate _version.py in the new build/ directory and replace
             # it with an updated value
             if cfg.versionfile_build:
-                target_versionfile = os.path.join(self.build_lib,
-                                                  cfg.versionfile_build)
+                target_versionfile = os.path.join(
+                    self.build_lib, cfg.versionfile_build
+                )
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
+
     cmds["build_py"] = cmd_build_py
 
-    if 'build_ext' in cmds:
-        _build_ext = cmds['build_ext']
+    if "build_ext" in cmds:
+        _build_ext = cmds["build_ext"]
     else:
         from setuptools.command.build_ext import build_ext as _build_ext
 
     class cmd_build_ext(_build_ext):
         def run(self):
             root = get_root()
             cfg = get_config_from_root(root)
@@ -1907,27 +1971,32 @@
                 # As in place builds will already have a _version.py
                 # in the module dir, we do not need to write one.
                 return
             # now locate _version.py in the new build/ directory and replace
             # it with an updated value
             if not cfg.versionfile_build:
                 return
-            target_versionfile = os.path.join(self.build_lib,
-                                              cfg.versionfile_build)
+            target_versionfile = os.path.join(
+                self.build_lib, cfg.versionfile_build
+            )
             if not os.path.exists(target_versionfile):
-                print(f"Warning: {target_versionfile} does not exist, skipping "
-                      "version update. This can happen if you are running build_ext "
-                      "without first running build_py.")
+                print(
+                    f"Warning: {target_versionfile} does not exist, skipping "
+                    "version update. This can happen if you are running build_ext "
+                    "without first running build_py."
+                )
                 return
             print("UPDATING %s" % target_versionfile)
             write_to_version_file(target_versionfile, versions)
+
     cmds["build_ext"] = cmd_build_ext
 
     if "cx_Freeze" in sys.modules:  # cx_freeze enabled?
         from cx_Freeze.dist import build_exe as _build_exe
+
         # nczeczulin reports that py2exe won't like the pep440-style string
         # as FILEVERSION, but it can be used for PRODUCTVERSION, e.g.
         # setup(console=[{
         #   "version": versioneer.get_version().split("+", 1)[0], # FILEVERSION
         #   "product_version": versioneer.get_version(),
         #   ...
 
@@ -1940,25 +2009,29 @@
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
                 _build_exe.run(self)
                 os.unlink(target_versionfile)
                 with open(cfg.versionfile_source, "w") as f:
                     LONG = LONG_VERSION_PY[cfg.VCS]
-                    f.write(LONG %
-                            {"DOLLAR": "$",
-                             "STYLE": cfg.style,
-                             "TAG_PREFIX": cfg.tag_prefix,
-                             "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                             "VERSIONFILE_SOURCE": cfg.versionfile_source,
-                             })
+                    f.write(
+                        LONG
+                        % {
+                            "DOLLAR": "$",
+                            "STYLE": cfg.style,
+                            "TAG_PREFIX": cfg.tag_prefix,
+                            "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                            "VERSIONFILE_SOURCE": cfg.versionfile_source,
+                        }
+                    )
+
         cmds["build_exe"] = cmd_build_exe
         del cmds["build_py"]
 
-    if 'py2exe' in sys.modules:  # py2exe enabled?
+    if "py2exe" in sys.modules:  # py2exe enabled?
         try:
             from py2exe.setuptools_buildexe import py2exe as _py2exe
         except ImportError:
             from py2exe.distutils_buildexe import py2exe as _py2exe
 
         class cmd_py2exe(_py2exe):
             def run(self):
@@ -1969,63 +2042,70 @@
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
                 _py2exe.run(self)
                 os.unlink(target_versionfile)
                 with open(cfg.versionfile_source, "w") as f:
                     LONG = LONG_VERSION_PY[cfg.VCS]
-                    f.write(LONG %
-                            {"DOLLAR": "$",
-                             "STYLE": cfg.style,
-                             "TAG_PREFIX": cfg.tag_prefix,
-                             "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                             "VERSIONFILE_SOURCE": cfg.versionfile_source,
-                             })
+                    f.write(
+                        LONG
+                        % {
+                            "DOLLAR": "$",
+                            "STYLE": cfg.style,
+                            "TAG_PREFIX": cfg.tag_prefix,
+                            "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                            "VERSIONFILE_SOURCE": cfg.versionfile_source,
+                        }
+                    )
+
         cmds["py2exe"] = cmd_py2exe
 
     # sdist farms its file list building out to egg_info
-    if 'egg_info' in cmds:
-        _egg_info = cmds['egg_info']
+    if "egg_info" in cmds:
+        _egg_info = cmds["egg_info"]
     else:
         from setuptools.command.egg_info import egg_info as _egg_info
 
     class cmd_egg_info(_egg_info):
         def find_sources(self):
             # egg_info.find_sources builds the manifest list and writes it
             # in one shot
             super().find_sources()
 
             # Modify the filelist and normalize it
             root = get_root()
             cfg = get_config_from_root(root)
-            self.filelist.append('versioneer.py')
+            self.filelist.append("versioneer.py")
             if cfg.versionfile_source:
                 # There are rare cases where versionfile_source might not be
                 # included by default, so we must be explicit
                 self.filelist.append(cfg.versionfile_source)
             self.filelist.sort()
             self.filelist.remove_duplicates()
 
             # The write method is hidden in the manifest_maker instance that
             # generated the filelist and was thrown away
             # We will instead replicate their final normalization (to unicode,
             # and POSIX-style paths)
             from setuptools import unicode_utils
-            normalized = [unicode_utils.filesys_decode(f).replace(os.sep, '/')
-                          for f in self.filelist.files]
 
-            manifest_filename = os.path.join(self.egg_info, 'SOURCES.txt')
-            with open(manifest_filename, 'w') as fobj:
-                fobj.write('\n'.join(normalized))
+            normalized = [
+                unicode_utils.filesys_decode(f).replace(os.sep, "/")
+                for f in self.filelist.files
+            ]
+
+            manifest_filename = os.path.join(self.egg_info, "SOURCES.txt")
+            with open(manifest_filename, "w") as fobj:
+                fobj.write("\n".join(normalized))
 
-    cmds['egg_info'] = cmd_egg_info
+    cmds["egg_info"] = cmd_egg_info
 
     # we override different "sdist" commands for both environments
-    if 'sdist' in cmds:
-        _sdist = cmds['sdist']
+    if "sdist" in cmds:
+        _sdist = cmds["sdist"]
     else:
         from setuptools.command.sdist import sdist as _sdist
 
     class cmd_sdist(_sdist):
         def run(self):
             versions = get_versions()
             self._versioneer_generated_versions = versions
@@ -2039,16 +2119,18 @@
             cfg = get_config_from_root(root)
             _sdist.make_release_tree(self, base_dir, files)
             # now locate _version.py in the new base_dir directory
             # (remembering that it may be a hardlink) and replace it with an
             # updated value
             target_versionfile = os.path.join(base_dir, cfg.versionfile_source)
             print("UPDATING %s" % target_versionfile)
-            write_to_version_file(target_versionfile,
-                                  self._versioneer_generated_versions)
+            write_to_version_file(
+                target_versionfile, self._versioneer_generated_versions
+            )
+
     cmds["sdist"] = cmd_sdist
 
     return cmds
 
 
 CONFIG_ERROR = """
 setup.cfg is missing the necessary Versioneer configuration. You need
@@ -2100,36 +2182,43 @@
 
 
 def do_setup():
     """Do main VCS-independent setup function for installing Versioneer."""
     root = get_root()
     try:
         cfg = get_config_from_root(root)
-    except (OSError, configparser.NoSectionError,
-            configparser.NoOptionError) as e:
+    except (
+        OSError,
+        configparser.NoSectionError,
+        configparser.NoOptionError,
+    ) as e:
         if isinstance(e, (OSError, configparser.NoSectionError)):
-            print("Adding sample versioneer config to setup.cfg",
-                  file=sys.stderr)
+            print(
+                "Adding sample versioneer config to setup.cfg", file=sys.stderr
+            )
             with open(os.path.join(root, "setup.cfg"), "a") as f:
                 f.write(SAMPLE_CONFIG)
         print(CONFIG_ERROR, file=sys.stderr)
         return 1
 
     print(" creating %s" % cfg.versionfile_source)
     with open(cfg.versionfile_source, "w") as f:
         LONG = LONG_VERSION_PY[cfg.VCS]
-        f.write(LONG % {"DOLLAR": "$",
-                        "STYLE": cfg.style,
-                        "TAG_PREFIX": cfg.tag_prefix,
-                        "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                        "VERSIONFILE_SOURCE": cfg.versionfile_source,
-                        })
+        f.write(
+            LONG
+            % {
+                "DOLLAR": "$",
+                "STYLE": cfg.style,
+                "TAG_PREFIX": cfg.tag_prefix,
+                "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                "VERSIONFILE_SOURCE": cfg.versionfile_source,
+            }
+        )
 
-    ipy = os.path.join(os.path.dirname(cfg.versionfile_source),
-                       "__init__.py")
+    ipy = os.path.join(os.path.dirname(cfg.versionfile_source), "__init__.py")
     if os.path.exists(ipy):
         try:
             with open(ipy, "r") as f:
                 old = f.read()
         except OSError:
             old = ""
         module = os.path.splitext(os.path.basename(cfg.versionfile_source))[0]
```

