# Problem

## Introduction

Proteins are the workhorses of the cell. They are the building blocks of cellular infrastructure, they regulate gene expression, control the cell cycle, transport molecules, transduce signals, trigger immune responses, and catalyze essential biochemical reactions. The ability of proteins to take on such a staggering diversity of functions is critical to life’s survival. It is also the reason proteins are used in such a wide range of industrial and therapeutic applications.

A protein’s function is encoded in its amino acid sequence, a molecular word constructed from an alphabet of twenty letters. Genetic changes, such as DNA mutations, that alter a protein’s amino acid sequence can impact its function. Such changes can be beneficial to an organism, such as those that increase protein thermostability, which can provide an adaptive advantage in a warming world. Others are beneficial for industrial and therapeutic applications, such as those that increase the catalytic efficiency of an enzymatic reaction, which can enhance biofuel production, or those that confer cellular specificity to an antibody, which can improve the efficacy of immunotherapeutics. Others still are flat-out detrimental, leading to developmental disorders, disease, or death. Understanding how mutations influence protein function is therefore important in many scientific disciplines, including evolutionary biology, protein engineering, and drug design.

## Deep Mutational Scanning

Recent technological advances have facilitated the experimental interrogation of mutation on protein function at unprecedented resolution. For example, deep mutational scanning experiments leverage massively-parallel phenotypic screens and high-throughput DNA sequencing to provide a functional readout for a large number of single-letter changes to a protein’s amino acid sequence. Often, these include all single-letter changes, such that the data comprise a readout for 19L mutations, where L is the length of the amino acid sequence. Some studies even describe the functional effects of mutations in combination, such as pairs and triplets. Despite their impressive scale, these data comprise only a vanishingly small fraction of the 20L possible amino acid sequence variants of any protein. An important challenge is therefore to leverage data from deep mutational scanning experiments to make accurate predictions of the functional effects of mutations for which we do not yet have experimental data.

## Machine Learning

Central to overcoming this challenge is machine learning. In particular, large language models, such as those that power Chat-GPT, are increasingly being used to learn the language of molecules, including proteins. Rather than pre-training on text scraped from the web, they are pre-trained on hundreds of millions of amino acid sequences that span evolutionary diversity. The resulting representations, or embeddings, of amino acid sequences encode information about the evolutionary history, structure, and function of proteins. Importantly, proteins with very dissimilar amino acid sequences may have very similar representations, and vice versa. As such, these representations may prove more useful in predicting the functional effects of proteins than do the amino acid sequences themselves.

## The Task

Your task is to use the representations of protein sequences from a popular large language model called ESM to make predictions about the functional effects of mutations using data from deep mutational scanning experiments. 
