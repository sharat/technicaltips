If you notice, you won't able to see any changes in the sublime text font on changing the Default or user settings. As the note mentioned in the default settings, the platform specific settings file overrides the font face and size by default.
You can see this in `Preferences (<Platform>).sublime-settings` file.

On Windows you can locate this at 
`%APPDATA%\Sublime Text 2\Packages\Default\Preferences (Windows).sublime-settings`

for e.g. This is how you set `Source Code Pro` font for sublime text.
```
{
	"font_face": "Source Code Pro Light",
	"font_size": 10
}
```
