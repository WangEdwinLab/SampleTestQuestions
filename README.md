# Masking .vcf file based on given genome intervals
Use any development environment that you're familiar with and feel free to refer to API docs.

## Objective
The .vcf file contains single nucleotide variants(SNVs), one entry per line. Suppose that we're interested in some restricted reigions, provided in the other file, across the genome. Some SNVs need to be filtered out based on this criterion.

Please print the first 1000 lines that contain SNVs located *inside* at least one of the given intervals, i.e. a SNV fulfills left_boundary<=coordinate<=right_boundary will be considered acceptable.


## File formats
delimiter: \t

newline  : \n

comment  : #
- intervals.txt | chromosome, left_boundary, right_boundary

- vcf.vcf       | chromosome, coordinate, ID_for_this_mutation, before_mutation, after_mutation

(In both files, coordinates are ascending for each chromosome.)
