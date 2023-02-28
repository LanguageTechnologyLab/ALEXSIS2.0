
# ALEXSIS+: An IR Approach to Substitute Generation and Selection in Lexical Simplification
Lexical simplification (LS) automatically replaces words that are deemed difficult to understand for a given target population with simpler alternatives, whilst preserving the meaning of the original sentence. The TSAR-2022 shared task on LS provided participants with a multilingual lexical simplification test set. It contained nearly 1,200 complex words in English, Portuguese, and Spanish and presented multiple candidate substitutions for each complex word. The competition did not make training data available; therefore, teams had to use either off-the-shelf pre-trained large language models (LLMs) or out-domain data to develop their LS systems. As such, participants were unable to fully explore the capabilities of LLMs by re-training and/or fine-tuning them on in-domain data. To address this important limitation, we present ALEXSIS+, a multilingual dataset in the aforementioned three languages, and ALEXSIS++, an English monolingual dataset that together contains more than 50,000 unique sentences retrieved from news corpora and annotated with cosine similarities to the original complex word and sentence. Using these additional contexts, we are able to generate new high-quality candidate substitutions that improve LS performance on the TSAR-2022 test set regardless of the language or model. We make both ALEXSIS+ and ALEXSIS++ freely available to the research community.

## ALEXSIS+ & ALEXSIS++

ALEXSIS+ has a total of 12,831, 13,353, and 13,541 matched complex words in unique contexts for English, Spanish, and Portuguese, respectively. The larger ALEXSIS++ dataset contains matched complex words in 33,149 unique contexts only for English. Each dataset has the following nine headers separated by tab (\t).  

## Dataset Format
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
