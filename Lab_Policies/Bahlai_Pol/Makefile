all : Bahlai_policies_lab.pdf rm_files

# Assemblages des différentes parties de la charte de lab de Christie Bahlai
Bahlai_policies_lab.pdf: Code_of_conduct.pdf general_guidelines.pdf Project_completion.pdf
	pdfunite $^ $@

# Conversion en pdf du code de conduite
Code_of_conduct.pdf: Code_of_conduct.md
	pandoc $< -s -o $@

# Conversion en pdf des guide lines generales
general_guidelines.pdf: general_guidelines.md
	pandoc $< -s -o $@

# Conversion en pdf de la réalisation de projet
Project_completion.pdf: Project_completion.md
	pandoc $< -s -o $@

# Suppression des pdf inutiles
rm_files : Code_of_conduct.pdf general_guidelines.pdf Project_completion.pdf
	rm $^
