# Masking .vcf file based on given genome intervals
Use any development environment that you're familiar with and feel free to refer to API docs.


## File formats
delimiter: \t

newline  : \n

comment  : #
- intervals.txt | chromosome, left_boundary, right_boundary

- vcf.vcf       | chromosome, coordinate, ID_for_this_mutation, before_mutation, after_mutation

(In both files, coordinates are ascending for each chromosome.)
