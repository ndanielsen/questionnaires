QUESTIONNAIRES
======

Check the [example folder](https://github.com/saiki-gg/questionnaires/tree/master/example) as a reference.

**RULES:**

- A folder per questionnaire with the three required .json files
- "name" attribute -> lowercase, no spaces (use - instead) and in english
- Numbers allways as number, never as a string

**TODO:**
- Data loader to the DB
- Update data if the json are updated

**IDEAS:**
- Just launch a command that checks if the folder and the jsons are valid
- If the jsons aren't correct get some clear feedback about the error and in which line
- `node loader.js hexaco-100` will create/update the `hexaco-100` folder
- `node loader.js hexaco-100 production` will launch the script agains the production DB

