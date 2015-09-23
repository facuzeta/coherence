<h2>Coherence Algorithm</h2>

 
Coherence Algorithm used in *Automated analysis of free speech predicts psychosis onset in high-risk youths*
(<a href="http://www.nature.com/articles/npjschz201530?WT.mc_id=GOP_SCHZ_1508_201530">download the paper</a>) to study the speech coherence level. For now, the algorithm works in English but it is very easy to adapt into others languages.

<h2> On-line use</h2>
It is available to use online in the site: http://speech-tools.liaa.dc.uba.ar/coherence/


<h2> Install </h2>
The easy way to install is using pip, doing:

pip install git+https://github.com/facuzeta/coherence/

It takes some time becouse it has to download the trained models ( more than > 30 MB)

<h2> Example </h2>

After install...

```
import coherence

some_large_text= "The campaign brought ... I began by making up my mind..."

coh = coherence.coherenceAnalisys()
coh.analysis_text(some_large_text)
res = coh.analysis_text(some_large_text) 
```
*res* is the dictionary with the statistics, you can see the result using the on-line app http://speech-tools.liaa.dc.uba.ar/coherence/

<h2> How does it work? </h2>
<img src="http://speech-tools.liaa.dc.uba.ar/coherence/media/coherence_analysis.png" width=600px/>
