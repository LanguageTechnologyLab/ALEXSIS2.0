# ALEXSIS+

ALEXSIS+ has a total of 12,831, 13,353, and 13,541 matched complex words in unique contexts for English, Spanish, and Portuguese, respectively. The larger ALEXSIS++ dataset contains matched complex words in 33,149 unique contexts only for English. Each dataset has the following nine headers separated by tab (\t).  



# Dataset Format
<table>
    
   <tr>
    <th>Header</th>
    <th>Description</th>
  </tr>
 
    
  <tr>
    <td><b>ID</b></td>
    <td>Instance id that is made up of the original instance id (e.g. 01) and the new additional context id. (e.g. 104): 01-104.</td>
  </tr>
    
   <tr>
    <td><b>ALEXSIS.CW</b></td>
    <td>The original complex word taken form ALEXSIS and used at TSAR-2022.</td>
  </tr>
    
  <tr>
    <td><b>ALEXSIS.Context</b></td>
    <td>The original context for the given complex word taken form ALEXSIS and used at TSAR-2022.</td>
  </tr>
    
  <tr>
    <td><b>Candidate.Subs@n</b></td>
    <td>The candidate substitutions generated using MLM on the instances provided by TSAR-2022.</td>
  </tr>
    
  <tr>
    <td><b>Additional.Context</b></td>
    <td>New additional context obtained from the CC-News dataset.</td>
  </tr>
    
  <tr>
    <td><b>Additional.Subs@n</b></td>
    <td>New additional candidate substitutions generated using MLM on the additional contexts taken from the CC-News dataset</td>
  </tr>
    
  <tr>
    <td><b>Sent.Sim</b></td>
    <td>The cosine similarities between the SBert sentence embedding of the additional context and the original context provided by TSAR-2022.</td>
  </tr>

  <tr>
    <td><b>Word.Sim</b></td>
  <td>The cosine similarities between the word embeddings of the additional candidate substitutions and the original complex word provided by TSAR-2022.</td>
  </tr>
     
  <tr>
    <td><b>Gold.Labels</b></td>
    <td>The original gold candidate substitutions provided by TSAR-2022.</td>
  </tr>    

</table>
