# hse_hw3_chromhmm
## Colab
[Ссылка на Colab](https://colab.research.google.com/drive/1IQP932OZE9tgE4FGZIPr1rw7EFuKfO2p?usp=sharing)
## Выборка данных
В работе анализируются гистоновые модификации клеточной линии K562

Гистоновая метка | Имя файла | Используемый файл
--- | --- | ---
H2AFZ | wgEncodeBroadHistoneK562H2azStdAlnRep1.bam | H2AFZ.bam
H3K27me3 | wgEncodeBroadHistoneK562H3k27me3StdAlnRep1.bam | H3K27me3.bam
H3K36me3 | wgEncodeBroadHistoneK562H3k36me3StdAlnRep1.bam | H3K36me3.bam
H3K4me1 | wgEncodeBroadHistoneK562H3k4me1StdAlnRep1.bam | H3K4me1.bam
H3K4me2 | wgEncodeBroadHistoneK562H3k4me2StdAlnRep1.bam | H3K4me2.bam
H3K4me3 | wgEncodeBroadHistoneK562H3k4me3StdAlnRep1.bam | H3K4me3.bam
H3K79me2 | wgEncodeBroadHistoneK562H3k79me2StdAlnRep1.bam | H3K79me2.bam
H3K9ac | wgEncodeBroadHistoneK562H3k9acStdAlnRep1.bam | H3K9ac.bam
H3K9me1 | wgEncodeBroadHistoneK562H3k9me1StdAlnRep1.bam | H3K9me1.bam
H3K9me3 | wgEncodeBroadHistoneK562H3k9me3StdAlnRep1.bam | H3K9me3.bam
Control | wgEncodeBroadHistoneK562ControlStdAlnRep1.bam | Control.bam
## HTML отчет CromHMM

Предмет анализа | График
--- | ---
Fold Enrichment overlap | ![](/ChromHMM_data/A549_10_overlap.png)
Fold Enrichment TES neighborhood | ![](/ChromHMM_data/A549_10_RefSeqTES_neighborhood.png)
Fold Enrichment TSS neighborhood | ![](/ChromHMM_data/A549_10_RefSeqTSS_neighborhood.png)
Emission Parameters | ![](/ChromHMM_data/emissions_10.png)
Transition parameters | ![](/ChromHMM_data/transitions_10.png)
