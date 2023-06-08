## Welcome to HiFiSLP Homepage
Generating photo-realistic sign language videos in any style from text has significant social implications.
However, most existing methods can only generate average signer style under-articulated skeletal pose sequences.
In this work, we propose HiFiSLP, a high-fidelity sign language production (SLP) framework, which can generate expressive sign language videos consistent with different signer styles.
Specifically, we designed a motion style encoder that extracts the signer's style features from several seconds of reference videos and encodes them as fixed-dimensional embedding vectors.
In addition, we propose DiffSigner, a novel sign language motion generator based on the diffusion probabilistic model, which can synthesize high-fidelity sign language motions based on text, style embedding.
It consists of a mixed linguistic encoder for enhancing generation quality and faithfulness, as well as a lightweight generation backbone network.
We utilize a video rendering network based on generative adversarial networks to render the final sign language video.
The experimental results on two datasets indicate that our approach achieves better semantic preservation and high-fidelity generation of sign language videos compared to previous methods.
Compared to the previous best end-to-end continuous SLP method on the Phoenix-2014T dataset, HiFiSLP achieved an improvement of over 40% in BLEU-4 score for the back translation metric.