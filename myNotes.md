myNotes.md

# need to create a menu item

{
    // For upper-case output (#ABCDEF), set "color_upper_case" to true
    // For lower-case (#abcdef), use false
    "color_upper_case": true,
    
    // Set false to use the default windows colorpicker
    "win_use_new_picker": true

    // For rgba_unit need to add anotber setting
    ,"rgba_unit":	true
}


        if color:
            # Determine user preference for case of letters (default upper)
            s = sublime.load_settings("ColorPicker.sublime-settings")
            upper_case = s.get("color_upper_case", True)
            if upper_case:
                color = color.upper()
            else:
                color = color.lower()
