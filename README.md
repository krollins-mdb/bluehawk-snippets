# bluehawk-snippets README

This extension adds snippets for the [Bluehawk markup processor](https://mongodb-university.github.io/Bluehawk/).

## Features

`bluehawk-snippets` lets you quickly add Bluehawk tags by typing out triggers,
then letting VS Code autocomplete the tag for you.

### Triggers

Triggers usually consist of three letters, always beginning with a `b`, followed
by the first letter of the Bluhawk tag's name. In cases where there are
duplicates, the trigger may be longer.

| Trigger | Description |
|---------|-------------|
| bss     | Start a Bluehawk snippet block: `:snippet-start: <name-of-snippet>`. |
| bse     | End a Bluehawk snippet block: `:snippet-end:`. |
| bsf     | Create a full Bluehawk snippet block, with both `:snippet-start:` and `:snippet-end:`. |
| brs     | Start a Bluehawk replace block. |
| bre     | End a Bluehawk replace block: `:replace-end:`. |
| brf     | Create a full Bluehawk replace block. |
| bel     | Emphasize a single line: `:emphasize:`. |
| breml   | Remove a single line: `:remove:`. |
| brems   | Start a Bluehawk remove block: `:remove-start:`. |
| breme   | End a Bluehawk remove block: `:remove-end:`. |
| bremf   | Create a full Bluehawk remove block, with both `:remove-start:` and `:remove-end:`. |
| bul     | Uncomment a single line: `:uncomment:`. |
| bus     | Start a Bluehawk uncomment block: `:uncomment-start:`. |
| bue     | End a Bluehawk uncomment block: `:uncomment-end:`. |
| buf     | Create a full Bluehawk uncomment block, with both `:uncomment-start:` and `:uncomment-end:`. |

### Dynamic comment format

Because Bluehawk tags are commented lines, this extension takes into account the
different comment formatting in languages that VS Code supports.

## Known issues

- Snippets in JSX don't work. Currently, snippets don't understand the JSX
contexts.
