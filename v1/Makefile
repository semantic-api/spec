include ../Makefile.in

SPECS=$(wildcard specs/*.schema.json)
.PHONY: $(SPECS)

check-specs:: $(SPECS)

$(SPECS):
	$(call check-jsonschema, $@, $(patsubst %.schema.json, %.sample.json, $@))

