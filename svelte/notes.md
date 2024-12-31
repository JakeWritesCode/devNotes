# Svelte Notes


## Superforms

### Superforms

> Problem: One particular form field does not seem to save. SuperDebug shows it as being set, but when it gets to serverside it is not there.

This is an annoying little problem. The answer is the forms ID's and names must match the name from the schema. It doesn't
seem to matter that you use `bind:value={whatever}`, at actual POST time it seems to pick up the values from the form 
like any old POST from request would. So the name must match.