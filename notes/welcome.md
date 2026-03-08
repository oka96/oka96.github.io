# Welcome to My Learning Notes

This website reads markdown files from the `notes/` folder.

## How to add a new note
- Create a new `.md` file inside `notes/`
- Add an entry in `notes/index.json` with:
  - `id`: unique URL hash
  - `title`: sidebar title
  - `file`: markdown file path

## Example
```json
{
  "id": "javascript-basics",
  "title": "JavaScript Basics",
  "file": "notes/javascript-basics.md"
}
```

Happy learning ✨
