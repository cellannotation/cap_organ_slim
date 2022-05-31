ROBOT = robot
URIBASE = http://purl.obolibrary.org/obo

all: cap_organ_slim.owl

IMP=true # Global parameter to bypass import generation
MIR=true # Global parameter to bypass mirror generation


# Generate release file by  merging in OWL from template
aba_uberon.owl: linkouts.owl
	robot merge --input $< --input tmp.owl annotate --ontology-iri $(URIBASE)/$@ convert -f ofn -o $@


# Compress for release to get below GitHub file size restrictions.
# aba-uberon.owl.gz: aba_uberon.owl
#	gzip $<

prepare_release: aba_uberon.owl
	cp $< ../../.


