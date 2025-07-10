# A Disaggregated Dataset on English Offensiveness Containing Spans

This is the data for the paper A Disaggregated Dataset on English Offensiveness Containing Spans. 

You can find the disaggregated labels in the file all_comments_disaggregated. 

Further, find the aggregated labels in the file all_comments_aggregated. 

The file splits_aggregated contains the splits used for the benchmarks in the paper. 

# Dataset description


## All_comments_disaggregated 

#### Index
The index in the Toxic Comment Classification Challenge, the source of the data

#### Comment
The text from the Toxic Comment Classification Challenge which was classified

#### Annotators not toxic
The annotator ids of the annotators who labelled the text as not toxic / not offensive 

#### Annotators insult
The annotator ids of the annotators who labelled the text to be an insult

#### Annotators hate
The annotator ids of the annotators who labelled the text to be hateful

#### Tags
The spans, the label of the spans and the annotators that annotated these spans

#### Jigsaw annotations
For comparison, we include the annotations from the original Toxic Comment Classification Challenge


## All_comments_aggregated & splits_aggregated
This version of the data contains the aggregated annotations we computed of the disaggregated annotations. We only list the elements that differ from the elements in all_comments_disaggregated.

#### Comment marked
The comment with the span annotations. We did not use this version of the comment for our benchmark.

#### Label
Denotes whether the aggregated label is Toxic / Offensive (1) or Not toxic / Not offensive (0)

#### Manually cleaned
Denotes whether the annotation in the aggregated dataset was manually cleaned (1) or not (0). It is 0 for all comments in this dataset since we did not manually clean it. 

#### Vulgar
Denotes whether the aggregated annotations contain a span labelled as vulgar (1) or not (0). We did not use this label for our evaluation.

#### Target group / Target individual / Target other
Denotes whether the aggregated annotations contain a span labelled as target_group / target_individual / target_other (1) or not (0). We did not use this label for our evaluation.

#### Label fine
The fine-grained label of the comment resulting from the labels toxic, vulgar, target_group, target_individual, target_other. We did not use this label for our evaluation.

#### Tags
The spans and the labels of the spans resulting from the aggregated spans of the disaggregated data. For spans labelled as vulgarity, the number of votes for the span to be vulgar is included.





