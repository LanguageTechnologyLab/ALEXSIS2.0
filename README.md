# ALEXSIS2.0

The ALEXIS+ and ALEXSIS++ datasets are divided into three sub-corpora corresponding to English (EN), Spanish (ES), and Portuguese (PT). Each dataset has the following nine headers separated by tab (\textbackslash t):  

<ul>
  <li><b>ID</b>: instance id that is made up of the original instance id (e.g. 01) and the new additional context id. (e.g. 104): 01-104.</li>
  <li><b>ALEXSIS.CW</b>: the original complex word taken form ALEXSIS and used at TSAR-2022.</li>
  <li><b>ALEXSIS.Context</b>: the original context for the given complex word taken form ALEXSIS and used at TSAR-2022.</li>
  <li><b>Candidate.Subs@n</b>: the candidate substitutions generated using MLM on the instances provided by TSAR-2022.</li>
  <li><b>Additional.Context</b>: new additional context obtained from the CC-News dataset.</li>
  <li><b>Additional.Subs@n</b>: new additional candidate substitutions generated using MLM on the additional contexts taken from the CC-News dataset.</li>
  <li><b>Sent.Sim</b>: the cosine similarities between the SBert sentence embedding of the additional context and the original context provided by TSAR-2022. </li>
  <li><b>Word.Sim</b>: : the cosine similarities between the word embeddings of the additional candidate substitutions and the original complex word provided by TSAR-2022.</li>
  <li><b>Gold.Labels</b>: the original gold candidate substitutions provided by TSAR-2022.  </li>
</ul>
