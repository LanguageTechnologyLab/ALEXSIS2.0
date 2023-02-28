# ALEXSIS2.0

ALEXSIS+ has a total of 12,831, 13,353, and 13,541 matched complex words in unique contexts for English, Spanish, and Portuguese, respectively. The larger ALEXSIS++ dataset contains matched complex words in 33,149 unique contexts only for English. Each dataset has the following nine headers separated by tab (\t):  


<table>
    
   <tr>
    <td>Header</td>
    <td>Description</td>
  </tr>
   <tr>
    <td>instance id that is made up of the original instance id (e.g. 01) and the new additional context id. (e.g. 104): 01-104.</td>
    <td>the original complex word taken form ALEXSIS and used at TSAR-2022.</td>
    <td> the original context for the given complex word taken form ALEXSIS and used at TSAR-2022.</td>
    <td>the candidate substitutions generated using MLM on the instances provided by TSAR-2022.</td>
    <td>new additional context obtained from the CC-News dataset.</td>
    <td>new additional candidate substitutions generated using MLM on the additional contexts taken from the CC-News dataset</td>
    <td>the cosine similarities between the SBert sentence embedding of the additional context and the original context provided by TSAR-2022.</td>
    <td>the cosine similarities between the word embeddings of the additional candidate substitutions and the original complex word provided by TSAR-2022.</td>
    <td>the original gold candidate substitutions provided by TSAR-2022.</td>
  </tr>
  <tr>
    <th><b>ID</b>:</th>
    <th><b>ALEXSIS.CW</b></th>
    <th><b>ALEXSIS.Context</b></th>
    <th><b>Candidate.Subs@n</b></th>
    <th><b>Additional.Context</b></th>
    <th><b>Additional.Subs@n</b></th>
    <th><b>Sent.Sim</b></th>
    <th><b>Word.Sim</b></th>
    <th><b>Gold.Labels</b></th>
  </tr>

</table>
