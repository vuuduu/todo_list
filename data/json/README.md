# Data Storage Format

## Directory Structure
`data/json`
-- README.md        # This file
-- groups.json      # Stores metadata about task groups
-- 1234.json        # Individual to-do list file (ID-based naming)
-- 5678.json

### groups.json Structure/contents
This file maintains mapping of group `IDs` to their names & associated to-do lists. Example below...
```
{
    "1": {
        "name": "partylist",
        "lists": ["1234", "5678"]
    },
    "2": {
        "name": "studylist",
        "lists": ["2222", "3333"]
    }
}
```

### To-Do List File Structure
Each to-do list stored in a separate JSON file named after its unqiue ID

**Example:**
```
{
    "id": "12345",
    "name": "Friends Giving List",
    "group": "1",
    "tasks": [
        {
            "name": "Buy Decoration",
            "status": "Todo",
            "note": "Go to Party City to get table cloth"
        },
        {
            "name": "Buy Mashed Potatoes",
            "status": "In Progress",
            "note": "Get mashed potatoes from Walmart"
        },
        {
            "name": "Get Soda",
            "status": "Todo",
            "note": "Buy Root Beer from Wegmans"
        }
    ]
}
```
