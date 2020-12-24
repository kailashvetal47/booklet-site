# CALL apoc.uuid.removeAll() yield label, installed, properties

it will add the uuid transaction handler for the provided label and uuidProperty, in case the UUID handler is already present it will be replaced by the new one: removes all previously added uuid handlers and returns uuids information. All the existing uuid properties are left as-is