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

Fold Enrichment overlap | Fold Enrichment TES neighborhood | Fold Enrichment TSS neighborhood | Emission Parameters | Transition parameters
--- | --- | --- | --- | ---
![](/ChromHMM_data/A549_10_overlap.png) |  ![](/ChromHMM_data/A549_10_RefSeqTES_neighborhood.png) | ![](/ChromHMM_data/A549_10_RefSeqTSS_neighborhood.png) |  ![](/ChromHMM_data/emissions_10.png) | ![](/ChromHMM_data/transitions_10.png)

# Визуализация данных в UCSC Genome Browser
![](UCSC_tracks.png)

## Таблица состояний

Номер | Эпигенетический тип | Ассоциированные гистоновые метки | Свойства
--- | --- | --- | ---
1 | Strong enhancer | H3K4m1 | H3K4m1 [ассоциирован](https://doi.org/10.1186/s12864-017-4353-7) с энхансером
2 | Weak/poised enhancer | H3K79m2 H3K4m1  | Часто после участков 1
3 | Weak Promoter | H3K79m2 | H3K79m2 [ассоциирован](https://www.sciencedirect.com/science/article/pii/S0092867412013554)
4 | Active Promoter | H3K4m2 H3K4m3 H3K9ac H3K79m2 | H3K4me3, H3K9ac [ассоциированы](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3842134/) с активным хроматином/промотором
5 | Insulator | H2AFZ H3K4m2 H3K4m3 H3K9ac |
6 | Weak Promoter | H2AFZ | H2AFZ [ассоциирован](https://pubmed.ncbi.nlm.nih.gov/33953180/) с промотором, неплохо встречается в гене
7 | Weak transcribed |  | Достаточно много в гене, но нет ассоциаций
8 | Heterochromatin |  | Большой процент в геноме, lamin
9 | Polycomb-repressed |  | По остаточному принципу
10 | Transcriptional elongation |  | Много в генах и в экзонах


