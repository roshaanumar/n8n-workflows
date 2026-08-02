# Splitting API Results Workflow

## Overview
This n8n workflow demonstrates how to retrieve data from a REST API and split an array response into individual items for further processing.

In this example, the workflow fetches Pokémon data from the PokeAPI and uses the Split Out node to convert the list of Pokémon into separate items.

## Workflow

1. Manual Trigger starts the workflow.
2. HTTP Request sends a GET request to the PokeAPI.
3. Split Out extracts the `results` array.
4. Each Pokémon becomes an individual item for downstream processing.

## Nodes Used

- Manual Trigger
- HTTP Request
- Split Out

## API Used

**PokeAPI**

Endpoint:
https://pokeapi.co/api/v2/pokemon

## Output

The workflow returns multiple individual items, each containing:

- Pokémon name
- Pokémon URL

Example:

```json
{
  "name": "bulbasaur",
  "url": "https://pokeapi.co/api/v2/pokemon/1/"
}
```

## Files Included

- `splitting-API-results.json` — n8n workflow
- `splitting-API-results.png` — Workflow screenshot

## Skills Demonstrated

- API integration
- HTTP GET requests
- JSON parsing
- Splitting array data
- Data transformation in n8n
