RESULT_DIR = ../results

all: cap_organ_slim.owl

# Generate release file by  merging in OWL from template
cap_organ_slim.owl: cap_helper.owl
	robot template --merge-before --input $< --template ../templates/template.csv annotate --annotation rdfs:comment "CAP Organ List Ontology" --output $(RESULT_DIR)/$@


