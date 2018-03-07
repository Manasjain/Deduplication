# Deduplication
Deduplicates dataset using csvdedupe.

1.) clone this repository to your machine.
1.) Create a python virtualenv for your project.	
	 Setting up virtualenv refer: http://docs.python-guide.org/en/latest/dev/virtualenvs/ 
2.) Activate virtualenv using below commands:
	 source project_name/bin/activate.
3.) change the directory to your cloned repository.
4.) csvdedupe takes a messy input file or STDIN pipe and identifies duplicates. Thus, provide an input file, field names, and output file:
	csvdedupe Deduplication/dataset.csv \  --field_names ln dob gn fn \    --output_file output.csv
5.) output.csv contains an additional column with cluster id.
