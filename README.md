# LightSeizureNet
LightSeizureNet (LSN), a lightweight and highly interpretable seizure detection model with dilated convolution, global average pooling and kernel-wise pruning for model compression. The LSN model can also provide fine-grained information such as the activated brain region and the frequency of brainwave during seizures for clinical diagnosis.

To show that the ECAMs obtained from the proposed LSN model can locate seizure onset zone, more examples of EEG recordings and the corresponding ECAMs are shown in Figs. 1 and 2.

![image](https://github.com/qiusiyuan23/LightSeizureNet/blob/main/Figures/Fig1.png)
Fig. 1. The EEG recordings and the corresponding ECAMs: A relatively easy-to-classify seizure case (chb14).

![image](https://github.com/qiusiyuan23/LightSeizureNet/blob/main/Figures/Fig2.png)
Fig. 2. The EEG recordings and the corresponding ECAMs: A difficult-to-classify seizure case (chb06).

A case that is relatively easy to classify is shown in Fig. 1. When the seizure starts, the epileptic waves occur at the electrodes near the prefrontal lobe of the patient (i.e. FP1-F7, FP1-F3, FP2-F4, FP2-F8). In ECAMs, the corresponding EEG channels turn red during the seizure, which indicates a high probability of epileptic waves. Therefore, the process of seizure is clearly shown by the ECAMs.

A case that is difficult to classify is shown in Fig. 2. In this case, high amplitude signals appear on various EEG channels before the seizure onset. However, these high amplitude signals do not lead to false alarm from ECAMs. When the seizure starts, the amplitude of the EEG signals is reduced. The high-frequency epileptic waves in F3-C3, F4-C4, and FZ-CZ have become the key to identify the seizures of this patient. This case shows that the ECAMs can distinguish between noise and epileptic waves, and correctly judge the epileptic status.

As shown in Figs. 1 and 2, when epileptic waves appear on some EEG channels, the corresponding channels in ECAMs react significantly. We can easily obtain the information of which EEG channel has epileptic waves. The sequence of ECAMs clearly shows the development of epilepsy, as illustrated in Figs. 1 and 2, which can help to find the seizure onset zone. Note that the proposed models do not require any prior knowledge. The LSN models automatically learn the characteristics of epileptic waves, identify epileptic waves, and accurately classify seizure states.
