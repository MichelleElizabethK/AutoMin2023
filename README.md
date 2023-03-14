# AutoMin2023
## Datasets
### Minuting datasets
- ELITR-minuting-corpus (small)
- Additional data generated by ChatGPT from transcripts?

### Relevant summarization datasets
- HuggingFace: https://huggingface.co/datasets?task_categories=task_categories:summarization

- CNN-Daily Mail
  - on HuggingFace 
  - CNN articles and summaries
- AMI Meeting Corpus
  - on HuggingFace 
  - meetings transcripts and summaries
- ICSI Meeting Corpus
  - not on HuggingFace
  - code to process: https://github.com/xcfcode/meeting_summarization_dataset
- Spotify Podcast Dataset
  - not on HuggingFace
- SAMSum Corpus
  - on HuggingFace
  - messenger-like conversations with summaries
- DialogSum
  - on HuggingFace
  - dialogues and summaries
- XSum Dataset
  - on HuggingFace
  - news articles and summaries
- MediaSum
  - on HuggingFace 
  - media interview transcripts and summaries
- OAGK/OAGKX
  - on Lindat
  - scientific articles with abstracts

- Info:
  - AMI and ICSI best but rather small
### ELITR Minuting Corpus
#### Minutes
- Original
  - Taken real time, some content of the meeting might be missing
- Generated
  - Taken later by independent annotator not present in the meeting
- Both can be used, both have some problems
#### Alignments
- They are aligned manually
- Can also be used for training, extract smaller pieces of transcripts and minutes that are properly aligned
- We can talk to Marie Hledikova, email or Wednesday at 10:00

## Models
### Pretrained summarization models
- https://huggingface.co/models?pipeline_tag=summarization&sort=downloads
- Relevant:
  - https://huggingface.co/vmarklynn/bart-large-cnn-icsi-ami-v3
  - https://huggingface.co/philschmid/flan-t5-base-samsum
  - https://huggingface.co/lidiya/bart-large-xsum-samsum

## Implementations
### Minuting Baseline Experiments
- Many work done, but not documented properly
- Some documentation: https://elitr.eu/deliverables/

### Additional Information related to the topic
- https://nlp-yang.github.io/Dialogue_Summarization.pdf
- https://www.catalyzex.com/s/Meeting%20Summarization


## TODO
1. Try some HuggingFace summarization pretrained models and finetune it on the minuting dataset
2. Download and analyze the various datasets