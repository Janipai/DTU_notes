QMD 0.6
SMP 0.7
CSD 0.4
OGT 0.6

todo:
M. Grimmer, R. Ramachandra, and C. Busch: Deep face age progression: A
survey. IEEE Access, 2021
• P. Drozdowski, C. Rathgeb, and C. Busch: Computational workload in bio-
metric identification systems: An overview. IET Biometrics, 2019
• T. Schlett et al.: Face image quality assessment: A literature survey. ACM
Computing Surveys (CSUR), 2021
![[Pasted image 20250605211645.png]]


![[Pasted image 20250607125754.png]]

21+3 papers

### A 3D Mask Presentation Attack Detection Method Based on Polarization Medium Wave Infrared Imaging

The existing 3D mask PAD methods are mainly divided into two categories: visible-based methods and infrared-based methods.

NIR imaging has a better performance than visible light imaging in the detection of 3D masks.

Firstly, Marcel et al. conducted a systematic study on the vulnerability of face
recognition systems to impersonation attacks based on custom-made silicone masks [23]. Furthermore,
they found that real human faces and 3D silicone masks showed significantly different low-order
statistics in the thermal domain, which means that thermal imaging can be used to detect 3D mask
presentation attacks [24].However, since the temperature information is easily changed by attackers,
resulting in a similar temperature reading for spoof faces and real faces, the expression of the thermal
infrared radiation information for real and fake faces will become similar, which may lead to the
degradation of the detection performance.
-

DoLP is a function of certain parameters, such as the
roughness, reflectivity, incidence angle and intensity contrast between the background and target.

Before and after wearing a 3D mask, the subject faces towards the imaging system, so
the incident angle θi can be regarded as a constant. (ii) The background is fixed, so the difference in
coefficient a can be seen as being caused by the difference in radiation intensity between a positive
and negative sample


what is assumed and what is not  derived in detail

figure 3 er lækker :)) (real vs fake for DoLP)

datasets - 3dmad and ms-face and the wide multi channel presentation attack

For face presentation attack detection, we believe that the larger the difference in the low-order
features of real and fake face images, the better the detection ability will be. In other words, the larger
the difference value D, the better the results will be for feature extraction using the PAD method. The
difference value D of real facial images and masked facial images is defined as:
![[Pasted image 20250611123556.png]]

o evaluate the PAD performance, this paper uses not only three old evaluation metrics (accuracy,
recall, and precision) but also two new metrics defined by the ISO/IEC 30107-3 standard, namely the
attack presentation classification error rate (APCER) and the bona fide presentation classification
(BPCER) error rate. Another metric which is also derived is the average classification error rate (ACER),
defined as (APCER+BPCER)/2, to summarize the overall performance of the PAD method as a single
number. The lower the ACER values, the better the performance [34].

polarization mwir imaging system er the shit

dette paper omhandler en problemstilling, overvejelser fra forskellige papers, de forskellige typer imaging systems, matematikken bag dem, et eksperiment med tilhørende data behandling for til sidst at konkludere

### A Study on Presentation Attack Detection in Thermal Infrared
The aim of this paper is to present outcomes of
investigations on the detection of various face presentation attacks in thermal infrared in various
conditions including thermal heating of masks and various states of subject

facial photographs, 3D-printed, custom flexible
3D-latex and silicone masks is provided - 2D paper-printed masks, 3D-printed masks, custom flexible latex full-face masks and custom
silicone masks

Attacks on facial sensors are presumably the easiest attacks to be performed
since they could be done using relatively cheap and accessible instruments including printed or
displayed photographs.

gør brug af 
- head-detection algorithm and deep neayral network-based classifiers
- cross-marterial validation

related works:
mange dataset
The most extensively explored PAIs include a printed
photo or replaying a video of a subject. However, more sophisticated PAIs are appearing, including
3D-printed masks, facial silicone masks or full-face latex masks

forskellige validerings methoder med deres tilhørende resultater i procent til at validere 3d masker er provided.

CNN for silicone masks

har fundet et paper der inkluderer briller

George et al. [ 13 ] proposed a multi-channel convolutional neural network (MC-CNN) tested
with grayscale, depth, infrared and thermal infrared images. The proposed method was reported
to obtain an average classification error rate (ACER) of 2.59% and 0.84% for thermal imaging and a
combination of grayscale, depth, infrared and thermal, respectively. This method obtains high results
when using different channels and should not be considered in a single-channel configuration

noise equivalent temperature difference (NETD) 

different types of camera and angles

landsmarks er forskellige for 3d printed masker for næse, mund og hals

forskellige conditions for billederne

2d paper giver ikke varme, men kan man detecte det alligevel?

et andet block diagram over pad

When presenting a facial photograph, printed or displayed in front of a thermal camera, the energy
radiated by the subject’s face is blocked by the PAI due to a negligible transmission of thermal energy
through paper. 

for object detection: YOLO v3 [28 ] as a single-shot detector (SSD) and Faster
R-CNN [29] as a region-proposal network (RPN

forskellige cnn og deep learning models

APCER og BPCER

bruger 10 fold fordi der ikke findes data nok?

latex mask was the hardest to detect as they were characterized with a high heat transmission and covered the entire head

he best performing methods connect various imaging modalities including the visible range,
depth, infrared and thermal infrared images. The multi-channel convolutional neural network
(MC-CNN) [13] achieved impressive results in a k-fold validation as well as in an unknown attack
scenario. This method was reported to obtain an ACER of 2.59% for thermal imaging and 0.84% for a
combination of grayscale, depth, infrared and thermal infrared, respectively.

The study also presents the impact of thermalization on PAD performance

### An Adaptive Spatio-temporal Global Sampling for Presentation Attack Detection

de forskellige typer af attacks i biometric systems (introduction)

One way to address the problem of domain shift consists
in using temporal feature learning. Existing works in this area
can be roughly categorized into three streams: (i) extracting
dynamic features through CNN network, e.g., using optical
flow, (ii) extracting Spatio-temporal features based on 3D
CNN, and (iii) learning long-range (sequential) data e.g.,
through Recurrent Neural Networks (RNN) [11]. 

snakker om objecter der bevæger sig, såsom head rotation and blinking in videos

the video is partitioned into a set of non-overlapping
segments. Then, local features are extracted independently
for each segment and their trajectory is evaluated to estimate
inter-frame motion. Finally, an aggregation function is used to
capture the gist of the dynamics and to encode the appearance
information of the video sequences into a compact image.

we propose to
use dense representation and utilize similarity transformation
that helps to minimize the black framing issue as shown
in Fig.1 and provides good coverage of image features for
improving the robustness of homography estimation

 ASGS is not only effective for photo
and replay attacks, but also outperform several state-of-the-art
silicone-based PAD methods [9], [8], [7], [7], [29], [30], [24]
under intra-dataset test environment

### # Boosting Face Presentation Attack Detection in Multi-Spectral Videos Through Score Fusion of Wavelet Partition Images

This research focuses on extending the usability and efficiency of
presentation attack detection algorithms in multiple spectrums
and ethnicity variations.

It
is observed that the proposed algorithm yields the best
results on almost all the databases using all three metrics
of APCER, BPCER, and EER. 

mindre fokus på silicone mask

### Face anti-spooﬁng from the perspective of data  sampling
(i) how differ-  
ently does CNN or RNN behave concerning spatial-temporal modelling  
of video data? and (ii) conduct comprehensive experiments and analysis  
to demonstrate that our approach is extensible, which can be plugged  
into different deep learning-based face PAD models

. However, we focus  
on evaluating the performance on the most challenging scenario, that  
is, cross-dataset (single-source) and multi-source scenarios in terms of  
HTER.

the results conﬁrm the effectiveness of our approach. In Table 3,  
we compare our results with those state-of-the-art methods [25–31]  
which focus on domain generalization settings. Based on the experimen-  
tal results, our method provides best performance on two benchmark  
databases (M and C) and a competitive performance on third dataset (I).

indholdte kun silicone i abstract

### Spoofing Deep Face Recognition with Custom Silicone Masks
This is the first
study to consider PAs performed using custom-made flexible
silicone masks

PAs fall into two categories: impersonation, where the
attacker attempts to impersonate the victim, and obfusca-
tion, where the attacker wishes to avoid being recognized.

rigid mask vs custom "blød" mask

R systems – VGG-Face [13], LightCNN [23]
and Facenet [17] – to mask-based PAs. The reason these spe-
cific CNN-FRs have been chosen for this study is that they
were shown to have very high FR performance, as well as
the highest vulnerability to 2D PAs [12].

this is the first FR-vulnerability study involving imperson-
ation PAs made using custom silicone masks. Our experi-
ments clearly show that the three CNN-FR methods are all
significantly vulnerable to custom-mask based PAs.


Der vel også andre der gør dette: Our first pre-processing step is to convert
the input RGB image to a gray-level image

discuss iapmr
![[Pasted image 20250624120434.png]]

de har taget de tre mest kendte cnn-fr, ny dataset med bona fide
viser sårbarheder på alle tre, som er 10 gasnge højere



future work
![[Pasted image 20250628075415.png]]
spoofing anti-face^



% duplicate
@article{george2019a,
  author = {George, Anjith and Mostaani, Zohreh and Geissenbuhler, David and Nikisins, Olegs and Anjos, Andre and Marcel, Sebastien},
  title = {Biometric face presentation attack detection with multi-channel convolutional neural network [arXiv]},
  language = {eng},
  format = {article},
  journal = {Arxiv},
  pages = {16 pp.},
  year = {2019}
}



@article{ieee2018a,
  author = {IEEE and Bhattacharjee, Sushil and Mohammadi, Amir and Marcel, Sebastien},
  title = {Spoofing Deep Face Recognition with Custom Silicone Masks},
  language = {eng},
  format = {article},
  journal = {2018 Ieee 9th International Conference on Biometrics Theory, Applications and Systems (btas)},
  pages = {7 pp.},
  year = {2018},
  issn = {24749680, 24749699},
  isbn = {1538671808, 1538671816, 9781538671801, 9781538671818, 1538671794, 9781538671795},
  publisher = {IEEE},
  doi = {10.1109/BTAS.2018.8698550}
}
