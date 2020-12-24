# CALL apoc.uuid.remove(label) yield label, installed, properties

it will add the uuid transaction handler for the provided label and uuidProperty, in case the UUID handler is already present it will be replaced by the new one: remove previously added uuid handler and returns uuid information. All the existing uuid properties are left as-is