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

Demos
---------------
We randomly selected 10 examples from the test set for demo display, and the random seed was set to 0. From left to right in the video, the ground truth, HiFiSLP generation results and Progressive Transformer generation results are shown respectively.

TEXT: morgen vormittag bleibt von dem ganzen starken regen noch hier im osten einige gewitter hängen in brandenburg starker regen in vorpommern und an der ostsee . GLOSS: MORGEN VOR MITTAG REGEN OST REGION REGEN BRAND BURG REGEN VOR POMMERN OST ID: test/11May_2010_Tuesday_heute-5990

<div><video controls="" preload="none" poster="poster">
<source id="mp4" src="./demo/11May_2010_Tuesday_heute-5990.mp4" type="video/mp4"></videos></div>

TEXT: an den temperaturen ändert sich wenig . GLOSS: TEMPERATUR WIE-IMMER ID: test/28February_2011_Monday_tagesschau-4988

<div><video controls="" preload="none" poster="poster">
<source id="mp4" src="./demo/28February_2011_Monday_tagesschau-4988.mp4" type="video/mp4"></videos></div>

TEXT: das ruhige trockene und zum teil recht freundliche hochdruckwetter begleitet uns auch in den nächsten tagen . GLOSS: RUHIG TROCKEN FREUNDLICH NAECHSTE BLEIBEN ID: test/07October_2010_Thursday_tagesschau-4129

<div><video controls="" preload="none" poster="poster">
<source id="mp4" src="./demo/07October_2010_Thursday_tagesschau-4129.mp4" type="video/mp4"></videos></div>

TEXT: richtung nordosten gibt es mehr wolken hier und da etwas regen . GLOSS: NORDOST MEHR WOLKE REGEN ID: test/26October_2009_Monday_tagesschau-1402

<div><video controls="" preload="none" poster="poster">
<source id="mp4" src="./demo/26October_2009_Monday_tagesschau-1402.mp4" type="video/mp4"></videos></div>

TEXT: der tag beginnt ganz im osten noch freundlich später zeigt sich dann auch im nordwesten häufiger die sonne sonst überwiegen die wolken . GLOSS: OST REGION ANFANG FREUNDLICH SPAETER NORDWEST AUCH SONNE SONST REGION WOLKE ID: test/04August_2011_Thursday_tagesschau-712

<div><video controls="" preload="none" poster="poster">
<source id="mp4" src="./demo/04August_2011_Thursday_tagesschau-712.mp4" type="video/mp4"></videos></div>

TEXT: dort morgen sommerlich heiße dreißig grad im emsland kühle sechzehn grad . GLOSS: MORGEN IX DREISSIG GRAD NORD REGION SECHSZEHN GRAD ID: test/25August_2010_Wednesday_tagesschau-8516

<div><video controls="" preload="none" poster="poster">
<source id="mp4" src="./demo/25August_2010_Wednesday_tagesschau-8516.mp4" type="video/mp4"></videos></div>

TEXT: besonders im osten deutschlands kann es ein wenig regnen oder schneien . GLOSS: BESONDERS OST DEUTSCH LAND MEHR REGEN ODER SCHNEE ID: test/18February_2011_Friday_tagesschau-6825

<div><video controls="" preload="none" poster="poster">
<source id="mp4" src="./demo/18February_2011_Friday_tagesschau-6825.mp4" type="video/mp4"></videos></div>

TEXT: im norden und im westen sowie in schauernähe stürmische böen . GLOSS: NORDWEST SCHAUER STURM KOMMEN ID: test/21November_2009_Saturday_tagesschau-4907

<div><video controls="" preload="none" poster="poster">
<source id="mp4" src="./demo/21November_2009_Saturday_tagesschau-4907.mp4" type="video/mp4"></videos></div>

TEXT: im bergland zum teil schnee an den alpen auch für längere zeit regen oder schnee . GLOSS: MEER SCHNEE SCHNEIEN DANN ALPEN REGEN SCHNEE SCHNEIEN ID: test/27November_2009_Friday_tagesschau-7341

<div><video controls="" preload="none" poster="poster">
<source id="mp4" src="./demo/27November_2009_Friday_tagesschau-7341.mp4" type="video/mp4"></videos></div>

TEXT: vor allem im süden können die gewitter unwetterartig ausfallen . GLOSS: PLOETZLICH IX GEWITTER KOENNEN WIE UNWETTER ID: test/03June_2011_Friday_tagesschau-7644

<div><video controls="" preload="none" poster="poster">
<source id="mp4" src="./demo/03June_2011_Friday_tagesschau-7644.mp4" type="video/mp4"></videos></div>



