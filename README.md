# Anki Quick Field Focus
Quickly focus on a particular field in the card browser using a keyboard shortcut. When trying to populate a particular field for many notes at once, it's helpful to have a shortcut which jumps direcly to a particular field from within the browser.

## Installation
Install from https://ankiweb.net/shared/info/1199312228

## Configuration

You do need to configure the addon to tell it which field in your for a given note type needs to be focused. After installing the addon, select it in the Anki addon manager, then click **Config**

For each shortcut that you need, add an entry which contains the note type, the keyboard shortcut, and the name of the field to focus on.

For example, I have a note type called **Chinese-Words**, and within that note type, I want to quickly focus on field **Example** using shortcut **Ctrl+T**

**Note: if you are a Mac user**: declaring a shortcut as **Ctrl+T** will allow you to use that shortcut while pressing **Command+T**.


    {
        "focus_field_shortcuts" : [
            {
                "note_type": "Chinese-Words",
                "shortcut": "Ctrl+T",
                "field": "Example"
            }
        ]
    }


Want to configure multiple field ? Just add them this way:

    {
        "focus_field_shortcuts" : [
            {
                "note_type": "Chinese-Words",
                "shortcut": "Ctrl+T",
                "field": "Example"
            },
            {
                "note_type": "Chinese-Words",
                "shortcut": "Ctrl+Q",
                "field": "Romanization"
            }            
        ]
    }
