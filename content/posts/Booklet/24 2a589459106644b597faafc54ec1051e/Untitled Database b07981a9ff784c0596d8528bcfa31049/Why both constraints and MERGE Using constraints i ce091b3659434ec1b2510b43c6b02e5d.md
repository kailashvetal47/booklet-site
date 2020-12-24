# Why both constraints and MERGE? Using constraints is different from using MERGE. Statements that create data in violation of the constraint will error, while statements that use MERGE will simply return existing values (no errors). If we use both, we avoid terminating our load statements due to constraint violations, and we also ensure we don’t accidentally create duplicates in adhoc queries.