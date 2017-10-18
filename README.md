# WTO calculation

file_Genes = Gene Expression Matrix (normalized).

How to run it from the shell:

java -jar -Xmx25G correlation.jar file_Genes file_Genes

java -jar -Xmx25G wto.jar folder_containing_output_of_correlation.jar
numbers_of_you_want_to_use

Hint: The -Xmx parameter controls how much memory the program can use.
Since the programs are using matrices don't be mean with that parameter.
Especially the wto consumes some memory because it stores the TFvsGenes,
GeneVsGene and the matrix product at runtime.
