SPECS=$(wildcard specs/*.schema.json)
.PHONY: $(SPECS)

all: $(SPECS)

$(SPECS):
	check-jsonschema --schemafile $@ $(patsubst %.schema.json, %.sample.json, $@)

