#Atomic 

Collection of atom plugins I use for dev

##Install

```apm install activate-power-mode advanced-open-file atom-material-ui autocomplete-modules autocomplete-paths color-picker editor-stats esformatter file-icons fold-functions gitignore-snippets highlight-selected imdone-atom language-gitignore language-javascript-jsx linter linter-eslint linter-flow mac-fix-path merge-conflicts minimap minimap-autohide minimap-bookmarks minimap-find-and-replace minimap-git-diff minimap-hide minimap-highlight-selected minimap-linter minimap-pigments minimap-selection npm-install pane-layout-plus pigments react-snippets regex-railroad-diagram regex-tester sort-lines terminal-plus tomorrow-night-eighties-syntax
```

##Plugin List

* [activate-power-mode](activate-power-mode)
* [advanced-open-file](advanced-open-file)
* [atom-material-ui](atom-material-ui)
* [autocomplete-modules](autocomplete-modules)
* [autocomplete-paths](autocomplete-paths)
* [color-picker](color-picker)
* [editor-stats](editor-stats)
* [esformatter](esformatter)
* [file-icons](file-icons)
* [fold-functions](fold-functions)
* [gitignore-snippets](gitignore-snippets)
* [highlight-selected](highlight-selected)
* [imdone-atom](imdone-atom)
* [language-gitignore](language-gitignore)
* [language-javascript-jsx](language-javascript-jsx)
* [linter](linter)
* [linter-eslint](linter-eslint)
* [linter-flow](linter-flow)
* [mac-fix-path](mac-fix-path)
* [merge-conflicts](merge-conflicts)
* [minimap](minimap)
* [minimap-autohide](minimap-autohide)
* [minimap-bookmarks](minimap-bookmarks)
* [minimap-find-and-replace](minimap-find-and-replace)
* [minimap-git-diff](minimap-git-diff)
* [minimap-hide](minimap-hide)
* [minimap-highlight-selected](minimap-highlight-selected)
* [minimap-linter](minimap-linter)
* [minimap-pigments](minimap-pigments)
* [minimap-selection](minimap-selection)
* [npm-install](npm-install)
* [pane-layout-plus](pane-layout-plus)
* [pigments](pigments)
* [react-snippets](react-snippets)
* [regex-railroad-diagram](regex-railroad-diagram)
* [regex-tester](regex-tester)
* [sort-lines](sort-lines)
* [terminal-plus](terminal-plus)
* [tomorrow-night-eighties-syntax](tomorrow-night-eighties-syntax)

##<a name="activate-power-mode"></a>[activate-power-mode](https://github.com/JoelBesada/activate-power-mode#readme) 

Activate POWER MODE to write your code in style.

### activate-power-mode atom package
A package for Atom to replicate the effects from [codeinthedark/editor](https://github.com/codeinthedark/editor). Available through the Atom package installer (https://atom.io/packages/activate-power-mode). 

Activate with <kbd>Ctrl</kbd>-<kbd>Alt</kbd>-<kbd>O</kbd> or through the command panel with `Activate Power Mode: Toggle`. Use the command again to deactivate. 

![activate-power-mode-0 4 0](https://cloud.githubusercontent.com/assets/688415/11615565/10f16456-9c65-11e5-8af4-265f01fc83a0.gif)

**For a list of power mode packages to other editors, check out [codeinthedark/awesome-power-mode](https://github.com/codeinthedark/awesome-power-mode).**
##<a name="advanced-open-file"></a>[advanced-open-file](https://github.com/Osmose/advanced-open-file#readme) 

Open and create files and directories easily. Type in a path (with autocomplete) and view directory contents.

### Advanced Open File

[![TravisCI Build Status](https://travis-ci.org/Osmose/advanced-open-file.svg)](https://travis-ci.org/Osmose/advanced-open-file)
[![AppVeyor Build status](https://ci.appveyor.com/api/projects/status/cwyb7f46dd1bbuxh/branch/master?svg=true)](https://ci.appveyor.com/project/Osmose/advanced-open-file/branch/master)



Advanced Open File is a package for helping Atom users to open files and folders
easily. It can also create new files and folders if they don't exist.

![Demo of plugin functionality](http://osmose.github.io/advanced-open-file/demo.gif)

Advanced Open File is fork of
[Advanced New File](https://github.com/Trudko/advanced-new-file), itself a fork
of [Fancy New File](https://github.com/rev087/fancy-new-file). Thanks to both
rev087 and Trudko for their work.

#### Usage

Hit `Cmd-Alt-O`/`Ctrl-Alt-O` to open the file list to the directory of the
current file. As you edit the path the file list will automatically show
matching files and directories. Hit `Tab` to autocomplete the path.

Relative paths are considered relative to the current project's first root
folder.

Hit `Enter` to open the file at the given path. If the file doesn't exist, a tab
will be opened that will save to that file. Any directories in the path that
don't exist will be created immediately upon hitting `Enter`.

You can also click on any entry in the file list to add it to the current path
(in the case of a directory) or to open it immediately (in the case of a file).
You can also use the `Up` and `Down` arrow keys to scroll through the list, and
`Enter` to select the currently-highlighted item.

If a directory has a plus symbol on the right side of its entry, clicking the
symbol will add it as a project directory. You can also add a highlighted
directory as a project directory using `Shift-Cmd-O`/`Ctrl-Alt-O`.

`Cmd-Z`/`Ctrl-Z` will undo changes made to the current path, such as
autocompletion or directory shortcuts.

#### Keybindings

Available commands for binding:

<dl>
  <dt><code>advanced-open-file:toggle</code></dt>
  <dd>Toggles the Advanced Open File dialog.</dd>

  <dt><code>core:confirm</code></dt>
  <dd>
    If a path has been selected with the cursor, open it. If no path is
    selected, open the current path in the input.
  </dd>

  <dt><code>advanced-open-file:confirm-selected-or-first</code></dt>
  <dd>
    Similar to <code>core:confirm</code>. If nothing is selected, select the
    first item in the list.
  </dd>

  <dt><code>core:cancel</code></dt>
  <dd>Close the Advanced Open File dialog.</dd>

  <dt><code>application:add-project-folder</code></dt>
  <dd>
    If a folder path has been selected with the cursor, add it as a project
    directory.
  </dd>

  <dt><code>advanced-open-file:autocomplete</code></dt>
  <dd>Attempts to autocomplete the current input.</dd>

  <dt><code>advanced-open-file:undo</code></dt>
  <dd>Undo changes to the current path.</dd>

  <dt><code>advanced-open-file:move-cursor-up</code></dt>
  <dd>Move the cursor/highlight for the currently selected file up.</dd>

  <dt><code>advanced-open-file:move-cursor-down</code></dt>
  <dd>Move the cursor/highlight for the currently selected file down.</dd>

  <dt><code>advanced-open-file:delete-path-component</code></dt>
  <dd>
    A more powerful version of <code>alt-backspace</code> that erases the a
    directory component in the miniEditor including the slash ('/').
  </dd>
</dl>

The following extra keybindings are included by default:

Action                                     | Extra Keys
------------------------------------------ | ------------------
`advanced-open-file:move-cursor-up`        | `Ctrl-p`, `Ctrl-i`
`advanced-open-file:move-cursor-down`      | `Ctrl-n`, `Ctrl-k`
`advanced-open-file:delete-path-component` | `Ctrl-l`

You can of course remap the keys however you wish. For example, add the
following to your keymap to map `Ctrl-x Ctrl-f` to toggle the dialog and
`Ctrl-j` to move the cursor down:

```cson
'atom-workspace':
  'ctrl-x ctrl-f': 'advanced-open-file:toggle'

'.advanced-open-file atom-text-editor':
  'ctrl-j': 'advanced-open-file:move-cursor-down'
```

#### Settings

<dl>
  <dt>Create directories</dt>
  <dd>
    Normally, when you attempt to open a path pointing to a directory that
    doesn't exist, an error beep sounds and nothing happens. When this setting
    is enabled, opening a non-existent directory will create it and show a
    notification confirming the creation.
  </dd>

  <dt>Create files instantly</dt>
  <dd>
    If checked, files are created immediately instead of on save if they don't
    exist.
  </dd>

  <dt>Default input value</dt>
  <dd>
    Determines what the default value in the path input is when the dialog is
    opened. Possible choices are nothing, the current project's root directory,
    or the directory of the currently-active file.
  </dd>

  <dt>Shortcuts for fast directory switching</dt>
  <dd>
    <p>
      When enabled, allows for quick directory switching when appending certain
      strings to a path that ends in a slash:
    </p>
    <ul>
      <li>
        Adding an extra slash (e.g. <code>/</code>) will switch to the
        filesystem root.
      </li>
      <li>
        Adding a tilde and a slash (e.g. <code>~/</code>) will switch to the
        current user's home directory.
      </li>
      <li>
        Adding a colon and a slash (e.g. <code>:/</code>) will switch to the
        current project's root directory.
      </li>
    </ul>
  </dd>
</dl>

#### Event Service

Other packages can subscribe to events to get notified when certain actions
happen in advanced-open-file. To do so, you'll need to consume the
`advanced-open-file-events` service:

##### `package.json`

```json
"consumedServices": {
  "advanced-open-file-events": {
    "versions": {
      "0.1.0": "consumeEventService"
    }
  }
}
```

##### Main Module

```coffeescript
{Disposable} = require 'atom'


module.exports =
  consumeEventService: (service) ->
    openDisposable = service.onDidOpenPath (path) ->
      console.log "Open: ###{path}"

    createDisposable = service.onDidCreatePath (path) ->
      console.log "Create: ###{path}"

    return new Disposable ->
      openDisposable.dispose()
      createDisposable.dispose()
```

##### `onDidOpenPath`

Triggered when a file is opened via advanced-open-file.

```coffeescript
service.onDidOpenPath (path) ->
  console.log "Open: ###{path}"
```

##### `onDidCreatePath`

Triggered when a file is created via advanced-open-file. Note that this is only
triggered when the "Create files instantly" preference is enabled. It does not
trigger when the preference is disabled and a new file is opened and then
subsequently saved.

```coffeescript
service.onDidCreatePath (path) ->
  console.log "Create: ###{path}"
```

#### Contributing

First, if you're interested in contributing, thank you! It's awesome that you
want to help!

The easiest way to contribute is to [file an issue][] with the bug you've found
or the new feature you want added. If you're interested in implementing the fix
for your request yourself, or fixing an issue submitted by someone else, read
on.

[file an issue]: https://github.com/Osmose/advanced-open-file/issues/new

##### Developer Setup

Setting up a development install is easy with [apm][]:

```sh
$ apm develop advanced-open-file /path/to/checkout
```

The command above will use Git to clone Advanced Open File to the
`/path/to/checkout` directory, download the dependencies, and create a symlink
in your `.atom` profile for the package.

Now, if you launch Atom with the `-d` flag, Atom will load the development
checkout of Advanced Open File (instead of the released version, if you have it
installed). Any changes you make to the code will be reflected if you use the
`Window: Reload` command in the [Command Palette][] to reload the editor.

That should be all you need to get started. Create a branch, write your changes,
and submit the branch as a pull request, and you should hear back shortly!

[apm]: https://github.com/atom/apm
[Command Palette]: https://atom.io/docs/latest/getting-started-atom-basics###command-palette

#### License

Licensed under the MIT License. See `LICENSE` for details.
##<a name="atom-material-ui"></a>[atom-material-ui](https://github.com/silvestreh/atom-material-ui#readme) 

A dark UI theme for Atom that follows Google's Material Design Guidelines

![](http://i.imgur.com/7C2H2mw.png)
---

A dynamic UI theme for Atom that (kinda) follows Google's Material Design Guidelines. Best with [Atom Material Syntax](https://github.com/silvestreh/atom-material-syntax). (Mostly) works with other dark syntax themes as it uses syntax colors for the UI. Light themes work too, but might not look as nice.

Inspired by Mattia Astorino's [SublimeText theme](https://github.com/equinusocio/material-theme).

#### Installation

Fire up a console and type:

`$ apm install atom-material-ui atom-material-syntax atom-material-syntax-light`

Or, inside Atom's settings select Install and then search for this package.

#### Configuration

Atom Material UI supports different accent colors. To change it, go to Settings > Themes and click the cog icon next to the theme selector.

![](http://i.imgur.com/JB2iA5m.png)

You'll find the color dropdown there.

#### Screenshot

Here's the obligatory screenshot. The toolbar on the left side is a package named [Tool-bar-main](https://atom.io/packages/tool-bar-main).

![](http://i.imgur.com/2jNgkR9.png)

Animated tabs! (these animations can be disabled from the theme's settings)

![](http://i.imgur.com/lUR3uRv.gif)

#### Light syntax theme variant

![](http://i.imgur.com/HkCKXxX.png)

#### Extra

![](http://i.imgur.com/0tHORB1.png)

You can download the redesigned icon from [dropbox](https://dl.dropboxusercontent.com/u/115930/Atom-MD-Icon.zip). It's a ZIP file containing multiple resolution PNGs, ICNS and ICO formats. Windows ICO converted by Akshit Tripathi.
##<a name="autocomplete-modules"></a>[autocomplete-modules](https://github.com/nkt/atom-autocomplete-modules#readme) 

Autocomplete for require/import statements

### Atom autocomplete for modules.
[![Current version](https://img.shields.io/apm/v/autocomplete-modules.svg)](https://atom.io/packages/autocomplete-modules)
[![Downloads](https://img.shields.io/apm/dm/autocomplete-modules.svg)](https://atom.io/packages/autocomplete-modules)

Autocomplete for require/import statements.

![Preview](https://cloud.githubusercontent.com/assets/3505878/7442538/9c1892cc-f11e-11e4-8070-3fa8b79beefc.gif)

License
-------
[![MIT License](https://img.shields.io/apm/l/autocomplete-modules.svg)](LICENSE)
##<a name="autocomplete-paths"></a>[autocomplete-paths](https://github.com/atom-community/autocomplete-paths#readme) 

Adds path autocompletion to autocomplete+

### autocomplete+ paths suggestions [![Build Status](https://travis-ci.org/atom-community/autocomplete-paths.svg?branch=master)](https://travis-ci.org/atom-community/autocomplete-paths)

[![Gitter](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/atom-community/autocomplete-paths?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

[View the changelog](https://github.com/atom-community/autocomplete-paths/blob/master/CHANGELOG.md)

Adds path autocompletion to autocomplete+

![autocomplete-paths](http://s1.directupload.net/images/140411/p5kvife6.gif)

#### Installation

You can install autocomplete-paths using the Preferences pane.

**Please make sure you have autocomplete-plus installed as well**
##<a name="color-picker"></a>[color-picker](https://github.com/thomaslindstrom/color-picker) 

Right click or press CMD-SHIFT-C/CTRL-ALT-C to open it.

### A Color Picker for Atom

Right click and select `Color Picker`, or hit `CMD-SHIFT-C`/`CTRL-ALT-C` to open it. Currently reads `HEX`, `HEXa`, `RGB`, `RGBa`, `HSL`, `HSLa`, `HSV`, `HSVa`, `VEC3` and `VEC4` colors – and is able to convert between the formats.

It also inspects `Sass` and `LESS` color variables. Just open the `Color Picker` with the cursor at a variable and it'll look up the definition for you. From there, you can click the definition and go directly to where it's defined.

#### Preview

![Color Picker in action](https://github.com/thomaslindstrom/color-picker/raw/master/preview.gif)

#### Settings

Open `Atom Settings`, go to `Packages` in the left hand sidebar, and press `Settings` on `color-picker` to open the list of settings available for the Color Picker.

- **Abbreviate Color Values:** If possible, abbreviate color values, like for example “0.3” to “.3”,  “###ffffff” to “###fff” and “rgb(0, 0, 0)” to “rgb(0,0,0)”.
- **Automatically Replace Color:** Replace selected color automatically on change. Works well with as-you-type CSS reloaders.
- **Preferred Color Format:** On open, the Color Picker will show a color in this format.
- **Serve a random color on open:** If the Color Picker doesn't get an input color, it serves a completely random color.
- **Trigger key:** Decide what trigger key should open the Color Picker. `CMD-SHIFT-{TRIGGER_KEY}` and `CTRL-ALT-{TRIGGER_KEY}`. Requires a restart.
- **Uppercase Color Values:** If sensible, uppercase the color value. For example, “###aaa” becomes “###AAA”.

#### To do

- Selectable list of the current project color variables
##<a name="editor-stats"></a>[editor-stats](https://github.com/atom/editor-stats#readme) 

Display a graph of keyboard and mouse usage for the last 6 hours.

### Editor Stats package [![Build Status](https://travis-ci.org/atom/editor-stats.svg?branch=master)](https://travis-ci.org/atom/editor-stats)

View a graph of your mouse and keyboard activity for the last 6 hours.

The blue bar indicates the time of greatest activity.

You can toggle it using the `Editor Stats: Toggle` command from the command palette.

![](https://f.cloud.github.com/assets/671378/2262223/843b1172-9e57-11e3-9c60-8d28d542f39c.png)
##<a name="esformatter"></a>[esformatter](https://github.com/sindresorhus/atom-esformatter#readme) 

Beautify JavaScript

### esformatter

> Beautify JavaScript using [esformatter](https://github.com/millermedeiros/esformatter)

<img src="https://cloud.githubusercontent.com/assets/170270/4490970/2333d93a-4a33-11e4-9954-dffea0c5f528.gif" width="311">

*Issues with the output should be reported on the esformatter [issue tracker](https://github.com/millermedeiros/esformatter/issues).*


#### Install

```
$ apm install esformatter
```

Or, Settings → Install → Search for `esformatter`


#### Usage

Open the Command Palette and type `esformatter`.

Can also be run on just a selection. For example the code in a `<script>` tag.

There's a `Format On Save` option in the settings.


#### [Config](https://github.com/millermedeiros/esformatter###configuration)

Some [plugins](https://github.com/sindresorhus/atom-esformatter/blob/c5d0d550d94dd8c8caec4b7a5c0a72722d432e4d/package.json###L31-L43) are bundled. *PR welcome for more.*

Just add the ones you want to your config file:

```json
{
	"plugins": [
		"esformatter-braces"
	]
}
```


#### License

MIT © [Sindre Sorhus](http://sindresorhus.com)
##<a name="file-icons"></a>[file-icons](https://github.com/DanBrooker/file-icons) 

Assign file extension icons and colours for improved visual grepping

### If you've just updated and your icons are all messed up, please restart Atom before filing an issue.

Some of the underlying icon fonts have updated and rearranged their icons, a restart will fix this.

#### Installing
###### On the command line:
```ssh
apm install file-icons
```
###### On Atom:
Go to `Preferences > Install`, search for `file-icons` and install it.

### file-icons

Adds file specific icons to atom for improved visual grepping. Works with Tree View and Fuzzy Finder and Tabs.

![Screenshot](https://raw.githubusercontent.com/DanBrooker/file-icons/master/file-icons.png)

A number of icons and colours are provided by default for a range of common file types.
If you have file that you would like custom icons for you can easily add this yourself.

File Icons are now specified via css(less) only.

#### No Colours

Disable colours in the settings.

#### Unity Theme

By default the Unity theme hides icons, you can force to show the icons in the settings

### Customisation

The following css can be added to your user stylesheet to customise files with the .rb file extension.

```css
@import "packages/file-icons/styles/colors"; // to use the colours
@import "packages/file-icons/styles/icons";  // to use the defined icons
```

```css
@import "packages/file-icons/styles/items";
@{pane-tab-selector}, .icon-file-text {
  &[data-name$=".rb"]          { .medium-red;             } // Colours icon and filename
  &[data-name$=".rb"]:before   { .ruby-icon; .medium-red; } // Colours icon only
}
```

Folders
```css
@import "packages/file-icons/styles/items";
@{pane-tab-selector}, .icon-file-directory {
  &[data-name=".git"]:before { .git-icon; }
}
```

#### Icons
Icons are located at `./stylesheets/icons.less`. You can create a custom CSS class and express its code through `content: "\fxxx";`. Octicons is the default icon's class.

```css
.ruby-icon { content: "\f047"; }
```

#### Fonts
Some custom fonts are already provided
* [FontAwesome](http://fortawesome.github.io/Font-Awesome/)(`.fa`)
* [FontMfizz](http://mfizz.com/oss/font-mfizz)(`.mf`)
* [Icomoon](http://icomoon.io)(`.iconmoon`)
* [Devicons](http://vorillaz.github.io/devicons/)(`.devicons`)

```css
.coffee-icon { .fa; content: "\f0f4"; }
```

#### Colours

Colours are from the [Base16](https://github.com/chriskempson/base16) colour palette. CSS classes used to apply color follow its primary 8 (eight) colours and 3 (three) variants:

  * Red, Green, Yellow, Blue, Maroon, Purple, Orange, Cyan.
  * Light, Medium, Dark.

Medium is colour provided by Base16. Light is medium lightened 15%. Dark is medium darkened 15%. In order to "construct" a CSS class color, you provide its variant followed by a dash (-).

```css
.light-red;
.medium-blue;
.dark-maroon;
```

### Acknowledgments

Wouldn't have even tried to make this if it weren't for [sommerper/filetype-color](https://github.com/sommerper/filetype-color)
Also thanks to all the [contributors](https://github.com/DanBrooker/file-icons/graphs/contributors).
##<a name="fold-functions"></a>[fold-functions](https://github.com/robballou/atom-fold-functions#readme) 

Toggle folding on all functions

### Fold Functions

Folds functions within your code. Currently comes with a toggle, fold, and unfold option that will look for functions marked with 'meta.function'. Handy because it won't fold things like comments associated with functions.

![screenshot](http://robballou.com/i/fold.gif)

*Note: this currently folds only those functions it finds at a single indentation (e.g. it will fold the top level functions)*

Heavily inspired/influnced by [Fold Comments](https://atom.io/packages/fold-comments).

#### Autofolding

You can turn on the auto-folding feature with the following in your configuration file:

```coffescript
"fold-functions":
    autofold: true
    shortfileCutoff: 42
    autofoldGrammars: []
    autofoldIgnoreGrammars: ['SQL', 'CSV', 'JSON', 'CSON', 'Plain Text']
```

By default, this is setup to ignore files that are under 42 lines. This can be configured by changing the `shortfileCutoff` option to a larger or smaller number. If you wish to fold all files, even short ones, you can change this option to `0`.

Additionally, two new autofolding options have been added in 0.4.2:

1. `autofoldGrammars` allows you to specify grammar names for grammars you *want* to autofold. An empty list (which is the default), means everything is fair game to fold. That is except...
2. `autofoldIgnoreGrammars` allows you to specify grammar names for grammars you *do not want to autofold*. This fires after `autofoldGrammars` and does have a default value (see above).
##<a name="gitignore-snippets"></a>[gitignore-snippets](https://github.com/jefkoslowski/gitignore-snippets) 

Quickly create .gitignore files with templates from GitHub.

### Gitignore Snippets

Quickly create .gitignore files with templates from [GitHub](https://github.com/github/gitignore).

![demo](https://dl.dropboxusercontent.com/u/268400/gitignore-snippets.gif)

#### Usage

Prefix a template name (lowercase) with "gig-" and press tab.

```
gig-[template-name]
```

#### Examples

##### Node
```
gig-node
```

##### Rails
```
gig-rails
```

#### Table of all available snippets

You can find all available templates on https://github.com/github/gitignore.

| Snippet                  | Template             |
|--------------------------|----------------------|
| gig-actionscript         | Actionscript         |
| gig-ada                  | Ada                  |
| gig-agda                 | Agda                 |
| gig-android              | Android              |
| gig-appceleratortitanium | AppceleratorTitanium |
| gig-archives             | Archives             |
| gig-archlinuxpackages    | ArchLinuxPackages    |
| gig-autotools            | Autotools            |
| gig-bancha               | Bancha               |
| gig-bricxcc              | BricxCC              |
| gig-c                    | C                    |
| gig-c++                  | C++                  |
| gig-cakephp              | CakePHP              |
| gig-cfwheels             | CFWheels             |
| gig-chefcookbook         | ChefCookbook         |
| gig-clojure              | Clojure              |
| gig-cloud9               | Cloud9               |
| gig-cmake                | CMake                |
| gig-codeigniter          | CodeIgniter          |
| gig-commonlisp           | CommonLisp           |
| gig-composer             | Composer             |
| gig-concrete5            | Concrete5            |
| gig-coq                  | Coq                  |
| gig-cvs                  | CVS                  |
| gig-dart                 | Dart                 |
| gig-darteditor           | DartEditor           |
| gig-delphi               | Delphi               |
| gig-dm                   | DM                   |
| gig-dreamweaver          | Dreamweaver          |
| gig-drupal               | Drupal               |
| gig-eagle                | Eagle                |
| gig-eclipse              | Eclipse              |
| gig-eiffelstudio         | EiffelStudio         |
| gig-elisp                | Elisp                |
| gig-emacs                | Emacs                |
| gig-ensime               | Ensime               |
| gig-episerver            | EPiServer            |
| gig-erlang               | Erlang               |
| gig-espresso             | Espresso             |
| gig-expressionengine     | ExpressionEngine     |
| gig-fancy                | Fancy                |
| gig-finale               | Finale               |
| gig-flexbuilder          | FlexBuilder          |
| gig-forcedotcom          | ForceDotCom          |
| gig-fuelphp              | FuelPHP              |
| gig-gcov                 | gcov                 |
| gig-go                   | Go                   |
| gig-gradle               | Gradle               |
| gig-grails               | Grails               |
| gig-gwt                  | GWT                  |
| gig-haskell              | Haskell              |
| gig-idris                | Idris                |
| gig-java                 | Java                 |
| gig-jboss                | Jboss                |
| gig-jekyll               | Jekyll               |
| gig-jetbrains            | JetBrains            |
| gig-joomla               | Joomla               |
| gig-jython               | Jython               |
| gig-kate                 | Kate                 |
| gig-kdevelop4            | KDevelop4            |
| gig-kohana               | Kohana               |
| gig-lazarus              | Lazarus              |
| gig-leiningen            | Leiningen            |
| gig-lemonstand           | LemonStand           |
| gig-lilypond             | Lilypond             |
| gig-linux                | Linux                |
| gig-lithium              | Lithium              |
| gig-magento              | Magento              |
| gig-matlab               | Matlab               |
| gig-maven                | Maven                |
| gig-mercurial            | Mercurial            |
| gig-meteor               | Meteor               |
| gig-modelsim             | ModelSim             |
| gig-monodevelop          | MonoDevelop          |
| gig-nanoc                | nanoc                |
| gig-netbeans             | NetBeans             |
| gig-node                 | Node                 |
| gig-notepadpp            | NotepadPP            |
| gig-objective-c          | Objective-C          |
| gig-ocaml                | OCaml                |
| gig-opa                  | Opa                  |
| gig-opencart             | OpenCart             |
| gig-oracleforms          | OracleForms          |
| gig-osx                  | OSX                  |
| gig-packer               | Packer               |
| gig-perl                 | Perl                 |
| gig-phalcon              | Phalcon              |
| gig-playframework        | PlayFramework        |
| gig-plone                | Plone                |
| gig-prestashop           | Prestashop           |
| gig-processing           | Processing           |
| gig-python               | Python               |
| gig-qooxdoo              | Qooxdoo              |
| gig-qt                   | Qt                   |
| gig-quartus2             | Quartus2             |
| gig-r                    | R                    |
| gig-rails                | Rails                |
| gig-redcar               | Redcar               |
| gig-rhodesrhomobile      | RhodesRhomobile      |
| gig-ros                  | ROS                  |
| gig-ruby                 | Ruby                 |
| gig-sass                 | Sass                 |
| gig-sbt                  | SBT                  |
| gig-scala                | Scala                |
| gig-scons                | SCons                |
| gig-scrivener            | Scrivener            |
| gig-sdcc                 | Sdcc                 |
| gig-seamgen              | SeamGen              |
| gig-sketchup             | SketchUp             |
| gig-slickedit            | SlickEdit            |
| gig-stella               | stella               |
| gig-sublimetext          | SublimeText          |
| gig-sugarcrm             | SugarCRM             |
| gig-svn                  | SVN                  |
| gig-symfony              | Symfony              |
| gig-symfony2             | Symfony2             |
| gig-symphonycms          | SymphonyCMS          |
| gig-tags                 | Tags                 |
| gig-target3001           | Target3001           |
| gig-tasm                 | Tasm                 |
| gig-tex                  | TeX                  |
| gig-textmate             | TextMate             |
| gig-textpattern          | Textpattern          |
| gig-turbogears2          | TurboGears2          |
| gig-typo3                | Typo3                |
| gig-umbraco              | Umbraco              |
| gig-unity                | Unity                |
| gig-vagrant              | Vagrant              |
| gig-vim                  | vim                  |
| gig-virtualenv           | VirtualEnv           |
| gig-visualstudio         | VisualStudio         |
| gig-vvvv                 | VVVV                 |
| gig-waf                  | Waf                  |
| gig-webmethods           | webMethods           |
| gig-windows              | Windows              |
| gig-wordpress            | WordPress            |
| gig-xcode                | Xcode                |
| gig-xilinxise            | XilinxISE            |
| gig-yeoman               | Yeoman               |
| gig-yii                  | Yii                  |
| gig-zendframework        | ZendFramework        |
##<a name="highlight-selected"></a>[highlight-selected](https://github.com/richrace/highlight-selected) 

Highlights the current word selected when double clicking

### Highlight Selected

[![Build Status](https://travis-ci.org/richrace/highlight-selected.svg?branch=master)](https://travis-ci.org/richrace/highlight-selected)

Double click on a word to highlight it throughout the open file.

This is something hacky I've put together as I missed the functionality that
Sublime gave.

Some code and has been taken from Atom's
  [find and replace](https://github.com/atom/find-and-replace) package

Please log any issues and pull requests are more than welcome!

![Gif in action](http://i.imgur.com/C5FnzzQ.gif)

Change the following CSS in your StyleSheet to change the colours to suit your
theme. Either set the light theme check box in settings to be able to toggle
between styles or just overwrite the default box/background.

```scss
atom-text-editor, atom-text-editor::shadow {
  // Box
  .highlights .highlight-selected .region {
    border-color: ###ddd;
  }
  // Background
  .highlights .highlight-selected.background .region {
    background-color: rgba(155, 149, 0, 0.6);
  }
  // Light theme box (set in settings)
  .highlights .highlight-selected.light-theme .region {
    border-color: rgba(255, 128, 64, 0.4);
  }
  // Light theme background (set in settings)
  .highlights .highlight-selected.light-theme.background .region {
    background-color: rgba(255, 128, 64, 0.2);
  }
}
```


### Issues and Todo

- Should we highlight symbols?
- Merge this feature in the
[find-and-replace](https://github.com/atom/find-and-replace) package
##<a name="imdone-atom"></a>[imdone-atom](https://github.com/imdone/imdone-atom#readme) 

A hackable task-board for TODOs, FIXMEs, HACKs, etc in your code.

// A HACK:4 ble task-board in your code.
----
##### You live in the code, your tasks should too!

![gifrecord_2015-11-12_085528](https://cloud.githubusercontent.com/assets/233505/11121461/9899fb14-891b-11e5-8aba-a4646f8b1428.gif)

[![apm](https://img.shields.io/apm/dm/imdone-atom.svg)](https://atom.io/packages/imdone-atom)
[![apm](https://img.shields.io/apm/v/imdone-atom.svg)]()

Developers are creative people and the text editor is their canvas.  For decades they've used TODO style code comments to track issues that almost never end up in issue tracking software.  imdone is a plugin for your favorite text editor that turns code comments into trackable issues.  It collects all TODO style comments in your project and organizes them in a drag and drop task-board that integrates with any web based issue tracking system.

imdone works best with todo.txt and markdown syntax.  See the [syntax guide at imdone-core](https://github.com/imdone/imdone-core###task-formats) for details.

Whats new!
----
- :zap: **Open all files for filtered tasks!**
- **Open task links in [intellij](https://www.jetbrains.com/products.html) family of products with imdone-atom and [imdone intellij plugin](https://plugins.jetbrains.com/plugin/8067)!**
- **[How To Write Plugins](https://github.com/imdone/imdone-atom/wiki/How-To-Write-Plugins) for imdone-atom**
- **Link your TODO comments to github issues.  Try the [imdone-atom-github](https://atom.io/packages/imdone-atom-github) plugin!**

Install
----
```
$ apm install imdone-atom
```
or open Atom and go to Preferences > Install and search for `imdone-atom`

Ignoring files
----
- Configuration setting  
You can ignore files with the "Exclude Vcs Ignored Paths" setting

- .imdoneignore  
[Glob](https://www.npmjs.com/package/glob) patterns in `.imdoneignore` will be matched against files and directories.  For example, if your project is in `/home/jesse/projects/imdone-atom` and your `.imdoneignore` looks like this, then all files and folders in `/home/jesse/projects/imdone-atom/lib` will be ignored.
```
lib
```
- .imdone/config.json  
imdone will also ignore files and folders that match a regex in the `.imdone/config.json`, `exclude` array.  The array is seeded with some common excludes on first run.

**IMPORTANT:** If your project is large (###files > 1000) consider adding an .imdoneignore file.

How To Link Code And Github Issues
----
Using [todo.txt metadata](https://github.com/imdone/imdone-core###metadata) in your tasks and a minor change to `.imdone/config.json`, you can link to external resources like github issues and profiles.  

- Add a `meta` attribute to `.imdone/config.json`  
```javascript
"meta": {
  "issue": {
    "urlTemplate": "https://github.com/imdone/imdone-core/issues/%s",
    "titleTemplate": "github issue ###%s"
  }
}
```

- Use `issue:[gh issue id]` as metadata in your tasks.  
<pre>
// &###35;BACKLOG:0 issue:27 Export TODOs
</pre>

- Your issue is linked to the comment!  
![gh-issue-imdone](https://cloud.githubusercontent.com/assets/233505/9595122/72542350-502a-11e5-87b3-a4eb49428b7c.png)

Look at [imdone/imdone-core###metadata](https://github.com/imdone/imdone-core###metadata) for more info.
##<a name="language-gitignore"></a>[language-gitignore](https://github.com/bsara/language-gitignore#readme) 

Syntax highlighting for .gitignore files in Atom

Syntax Highlighting for .gitignore Files in Atom
================================================

[![MIT License](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://github.com/bsara/language-gitignore/blob/master/LICENSE.md)


Adds syntax highlighting to .gitignore files in Atom.

For full list of supported formats for "Header Blocks", see the [header block samples page](https://github.com/bsara/language-gitignore/blob/master/samples-header-blocks.md).


![Screenshot](https://raw.githubusercontent.com/bsara/language-gitignore/master/screenshot.png)

***(Theme used in screenshot: "Oscuro Syntax"...which I have not yet finished but will soon)***
##<a name="language-javascript-jsx"></a>[language-javascript-jsx](https://github.com/subtlegradient/language-javascript-jsx#readme) 

JavaScript, ES6, ES7, React JSX, Flow, etc… by SubtleGradient of Facebook

### JavaScript, ES6, ES7, React JSX, Flow, etc…
#### by SubtleGradient of Facebook
##<a name="linter"></a>[linter](https://github.com/atom-community/linter#readme) 

A Base Linter with Cow Powers

Linter
======

[![Slack Badge](https://img.shields.io/badge/chat-atom.io%20slack-blue.svg?style=flat-square)](http://atom-slack.herokuapp.com/)
[![Build Status](https://img.shields.io/travis/atom-community/linter.svg?style=flat-square)](https://travis-ci.org/atom-community/linter)
[![Plugin installs!](https://img.shields.io/apm/dm/linter.svg?style=flat-square)](https://atom.io/packages/linter)
[![Package version!](https://img.shields.io/apm/v/linter.svg?style=flat-square)](https://atom.io/packages/linter)
[![Dependencies!](https://img.shields.io/david/atom-community/Linter.svg?style=flat-square)](https://david-dm.org/atom-community/linter)

Linter is a base linter provider for the Hackable [Atom Editor](http://atom.io).

It provides a top-level API to its consumer that allows them to visualize errors and other kind-of messages, easily.


![Preview](http://g.recordit.co/13RfmirPz2.gif)

###### How to / Installation

Install package through Atom or use CLI:

```
$ apm install linter
```

###### Available linters

[Full linters list](http://atomlinter.github.io/)

###### API Documentation

[Linter API wiki](https://github.com/atom-community/linter/wiki/Linter-API)

###### Performance Tuning

Is linter working slow for you? Try changing the interval of inline bubble or disabling it completely and/or try disabling Line tab.

###### Contribute

Stick to imposed codestyle:

* `$ npm i -g coffeelint eslint`
* `$ npm run lint`
##<a name="linter-eslint"></a>[linter-eslint](https://github.com/AtomLinter/linter-eslint#readme) 

Lint JavaScript on the fly, using ESLint

### linter-eslint
[![Build Status](https://travis-ci.org/AtomLinter/linter-eslint.svg)](https://travis-ci.org/AtomLinter/linter-eslint)
[![Dependency Status](https://david-dm.org/AtomLinter/linter-eslint.svg)](https://david-dm.org/AtomLinter/linter-eslint)

This linter plugin for [Linter](https://github.com/AtomLinter/Linter) provides
an interface to [eslint](http://eslint.org). It will be used with files that
have the "JavaScript" syntax.

#### Installation
```ShellSession
apm install linter-eslint
```

`linter-eslint` will look for a version of `eslint` local to your project and
use it if it's available. If none is found it will fall back to the version it
ships with.

Lets say you depend on a specific version of `eslint`, maybe it has unreleased
features, maybe it's just newer than what `linter-eslint` ships with. If
`your-project/node_modules/eslint` exists `linter-eslint` will be used.
This package requires an `eslint` of at least v1.0.0.

Note that if you do not have the `linter` package installed it will be installed
for you. If you are using an alternative `linter-*` consumer feel free to disable
the `linter` package.

#### Use with plugins

You have two options:

* Install locally to your project `eslint` and the plugin
  * `$ npm i --save-dev eslint [eslint-plugins]`

* Install globaly `eslint` and plugins
  * `$ npm i -g eslint [eslint-plugins]`
  * Activate `Use Global Eslint` package option
  * (Optional) Set `Global Node Path` with `$ npm config get prefix`


#### Contributing

If you would like to contribute enhancements or fixes, please do the following:

0. Fork the plugin repository
0. Hack on a separate topic branch created from the latest `master`
0. Commit and push the topic branch
0. Make a pull request
0. Welcome to the club!

Please note that modifications should follow these coding guidelines:

* Indent is 2 spaces
* Code should pass the `eslint` linter with the provided `.eslintrc`
* Vertical whitespace helps readability, don’t be afraid to use it

Thank you for helping out!
##<a name="linter-flow"></a>[linter-flow](https://github.com/AtomLinter/linter-flow) 

Lint JavaScript on the fly, using Flow

### linter-flow

Lightweight alternative to Facebook's Flow plugin for [facebook/flow](http://flowtype.org/).

![linter-demo](https://naman.s3.amazonaws.com/linter-flow-plus/linter-flow-plus.gif)

#### Installation

* Install [flow](http://flowtype.org/docs/getting-started.html###installing-flow)
* `flow init`
* `apm install linter-flow`

#### Settings

You can configure linter-flow by editing ~/.atom/config.cson (choose Open Your Config in Atom menu) or in Preferences:

```cson
'linter-flow':
  'executablePath': 'flow'
  'enableAll': false
```

* `executablePath`: Absolute path to the Flow executable on your system.
* `enableAll`: Typecheck all files, not just file containing `@flow`.

##### Why not X?

linter-flow is made to be a lightweight package that does one thing well.

1. A similarly named package: linter-flow-plus is now a mirror. The development happens for both packages in parallel.
2. IDE-flow works relatively well, but it doesn't lint on-the-fly and doesn't integrate with the linter package.
3. Nuclide has too many problems for now to be reliable. It also involves installing a large number of other packages.

Please Note: IDE-flow and Nuclide provide other features such as autocomplete, type definitions on hover etc. Please continue to use those services for those features. (possibly in addition to linter-flow)

##### Limitations

This linter currently does not support Hack. Though the linter just uses the flow-cli and hack support should be trivial to add, I'm not a Hack/PHP developer and I can't test that it actually works. I would welcome if someone was to add support for Hack to this package and test it.

#### Contributing

If you would like to contribute enhancements or fixes, please do the following:

1. Fork the plugin repository
2. Hack on a separate topic branch created from the latest `master`
3. Commit and push the topic branch
4. Make a pull request
5. Welcome to the club!

Please note that modifications should follow these coding guidelines:

* Indent is 2 spaces with `.editorconfig`
* Code should pass `eslint` linter with the provided `.eslintrc`
* Vertical whitespace helps readability, don’t be afraid to use it

**Thank you for helping out!**
##<a name="mac-fix-path"></a>[mac-fix-path](https://github.com/atom/mac-fix-path#readme) 

fix $PATH variable when running Atom from launcher

### mac-fix-path package

A short description of your package.

![A screenshot of your package](https://f.cloud.github.com/assets/69169/2290250/c35d867a-a017-11e3-86be-cd7c5bf3ff9b.gif)
##<a name="merge-conflicts"></a>[merge-conflicts](https://github.com/smashwilson/merge-conflicts#readme) 

Resolve git conflicts within Atom

### Merge Conflicts

[![Build Status](https://travis-ci.org/smashwilson/merge-conflicts.svg?branch=master)](https://travis-ci.org/smashwilson/merge-conflicts)

Resolve your git merge conflicts in Atom!

![conflict-resolution](https://raw.github.com/smashwilson/merge-conflicts/master/docs/conflict-resolution.gif)

This package detects the conflict markers left by `git merge` and overlays a set of controls for resolving each and navigating among them. Additionally, it displays your progress through a merge.

#### Features

 * Conflict resolution controls are provided for each detected conflict.
 * Choose your version, their version, combinations thereof, or arbitrary changes edited in place as a resolution.
 * Navigate to the next and previous conflicts in each file.
 * Track your progress through a merge with per-file progress bars and a file list.
 * Save and stage your resolved version of each file as it's completed.

#### Using

When `git merge` tells you that it couldn't resolve all of your conflicts automatically:

```
$ git merge branch
Auto-merging two
CONFLICT (content): Merge conflict in two
Auto-merging one
CONFLICT (content): Merge conflict in one
Automatic merge failed; fix conflicts and then commit the result.
```

Open Atom on your project and run the command `Merge Conflicts: Detect` (default hotkey: *alt-m d*). You'll see a panel at the bottom of the window describing your progress through the merge:

![merge progress](https://raw.github.com/smashwilson/merge-conflicts/master/docs/merge-progress.jpg)

Click each filename to visit it and step through the identified conflicts. For each conflict area, click "Use me" on either side of the change to accept that side as-is:

![conflict area](https://raw.github.com/smashwilson/merge-conflicts/master/docs/conflict-area.jpg)

Use the right-click menu to choose more advanced resolutions, like "ours then theirs", or edit any chunk by hand then click "use me" to accept your manual modifications. Once you've addressed all of the conflicts within a file, you'll be prompted to save and stage the changes you've made:

![save and stage?](https://raw.github.com/smashwilson/merge-conflicts/master/docs/were-done-here.jpg)

Finally, when *all* of the conflicts throughout the project have been dealt with, a message will appear to prompt you how to commit the resolution and continue on your way. :tada:

![onward!](https://raw.github.com/smashwilson/merge-conflicts/master/docs/merge-complete.jpg)

#### Events

The merge-conflicts plugin emits a number of events that other packages can subscribe to, if they wish. If you want your plugin to consume one, use code like the following:

```coffeescript
{CompositeDisposable} = require 'atom'

pkg = atom.packages.getActivePackage('merge-conflicts')?.mainModule
subs = new CompositeDisposable

subs.add pkg.onDidResolveConflict (event) ->

### ...

subs.dispose()
```

 * `onDidResolveConflict`: broadcast whenever a conflict is resolved. `event.file`: the absolute path of the file in which the conflict was found; `event.total`: the total number of conflicts in that file; `event.resolved`: the number of conflicts that are resolved, including this one.
 * `onDidStageFile`: broadcast whenever a file has been completed and staged for commit. `event.file`: the absolute path of the file that was staged.
 * `onDidQuitConflictResolution`: broadcast when you stop merging conflicts by clicking the quit button.
 * `onDidCompleteConflictResolution`: broadcast when all conflicts in all files have successfully been resolved.

#### Contributions

Pull requests are welcome, big and small! Check out the [contributing guide](./CONTRIBUTING.md) for details.
##<a name="minimap"></a>[minimap](https://github.com/atom-minimap/minimap#readme) 

A preview of the full source code.

[![Build Status](https://travis-ci.org/atom-minimap/minimap.svg?branch=master)](https://travis-ci.org/atom-minimap/minimap)
[![APM Version](https://img.shields.io/apm/v/minimap.svg)](https://atom.io/packages/minimap)
[![APM Downloads](https://img.shields.io/apm/dm/minimap.svg)](https://atom.io/packages/minimap)

### Minimap package

A preview of the full source code.

![Minimap Screenshot](https://github.com/atom-minimap/minimap/blob/master/resources/screenshot.png?raw=true)
<small>In the screenshot above the minimap-git-diff and minimap-highlight-selected plugins are activated.</small>

##### Installation

```
apm install minimap
```

##### Features

* Service-based Plugin API: Use the plugin generation command and start developing your plugin right away.
* Decoration API: Use the same API to manage `TextEditor` and `Minimap` decorations.
* Canvas-based Rendering: Simple, fast and flexible.
* Stand-alone Mode: Wants to display a preview of a text editor in your UIs, use a stand-alone version of the Minimap.

##### Available Plugins

Below is the list of available plugins so far:

Package|Description
---|---
[Auto-Hide](https://atom.io/packages/minimap-autohide)|Hides the Minimap while editing.
[Bookmarks](https://atom.io/packages/minimap-bookmarks)|Displays Atom bookmarks.
[Code Glance](https://atom.io/packages/minimap-codeglance)|Shows the code that's under the mouse cursor when hovering the Minimap.
[Cursor Line](https://atom.io/packages/minimap-cursorline)|Highlights the line with cursor.
[Find And Replace](https://atom.io/packages/minimap-find-and-replace)|Displays the search matches.
[Git Diff](https://atom.io/packages/minimap-git-diff)|Displays the file diff.
[Google-Repo-Diff-Minimap](https://atom.io/packages/google-repo-diff-minimap)|A Minimap binding for the [google-repo-diff](https://atom.io/packages/google-repo-diff) package and [google-repo](https://atom.io/packages/google-repo) package.
[GPool-Diff-Minimap](https://atom.io/packages/gpool-diff-minimap)|A minimap binding for the [gpool-diff](https://atom.io/packages/gpool-diff) package.
[Hide on inactive panes](https://atom.io/packages/minimap-hide)|Hide the Minimap when pane isn't focus.
[Highlight Selected](https://atom.io/packages/minimap-highlight-selected)|A Minimap binding for the [highlight-selected](http://atom.io/packages/highlight-selected) package.
[Linter](https://atom.io/packages/minimap-linter)|Displays [linter](https://atom.io/packages/linter) markers.
[Pigments](https://atom.io/packages/minimap-pigments)|Displays the [Pigments](https://atom.io/packages/pigments) colors.
[Selection](https://atom.io/packages/minimap-selection)|Display the buffer's selections.
[Split-Diff](https://atom.io/packages/minimap-split-diff)|A Minimap binding for the [split-diff](https://atom.io/packages/split-diff) package.

##### Settings

###### Auto Toggle

If checked the Minimap is toggled on at startup. `(default=true)`

###### Device Pixel Ratio Rounding

If checked the `devicePixelRatio` will be rounded using `Math.floor`. `(default=true)`

###### Display Code Highlights

If checked the code will be highlighted using the grammar tokens. `(default=true)`

`true`|`false`
---|---
![](https://github.com/atom-minimap/minimap/blob/master/resources/with-code-highlights.png?raw=true)| ![](https://github.com/atom-minimap/minimap/blob/master/resources/without-code-highlights.png?raw=true)

###### Display Minimap On Left

If checked the Minimap appears on the left side of editors, otherwise it appears on the right side. `(default=false)`

`true`|`false`
---|---
![](https://github.com/atom-minimap/minimap/blob/master/resources/minimap-on-left.png?raw=true)|![](https://github.com/atom-minimap/minimap/blob/master/resources/minimap-on-right.png?raw=true)

###### Char Height

The height of a character in the Minimap in pixels. `(default=2)`

`1px`|`2px`|`4px`
---|---|---
![](https://github.com/atom-minimap/minimap/blob/master/resources/1px-char-height.png?raw=true)|![](https://github.com/atom-minimap/minimap/blob/master/resources/2px-char-height.png?raw=true)|![](https://github.com/atom-minimap/minimap/blob/master/resources/4px-char-height.png?raw=true)

###### Char Width

The width of a character in the Minimap in pixels. `(default=1)`

`1px`|`2px`
---|---
![](https://github.com/atom-minimap/minimap/blob/master/resources/1px-char-width.png?raw=true)|![](https://github.com/atom-minimap/minimap/blob/master/resources/2px-char-width.png?raw=true)

###### Interline

The space between lines in the Minimap in pixels. `(default=1)`

`1px`|`2px`
---|---
![](https://github.com/atom-minimap/minimap/blob/master/resources/1px-interline.png?raw=true)|![](https://github.com/atom-minimap/minimap/blob/master/resources/2px-interline.png?raw=true)

###### Text Opacity

The opacity used to render the line text in the Minimap. `(default=0.6)`

`0.6`|`1`
---|---
![](https://github.com/atom-minimap/minimap/blob/master/resources/text-opacity-default.png?raw=true)|![](https://github.com/atom-minimap/minimap/blob/master/resources/text-opacity-1.png?raw=true)

##### Display Plugins Controls

If checked, the Minimap plugins can be activated/deactivated from the Minimap settings view and a quick settings dropdown will be available on the top right corner of the Minimap. `(default=true)`

**You need to restart Atom for this setting to be effective.**

![](https://github.com/atom-minimap/minimap/blob/master/resources/plugins-control.png?raw=true)

###### Minimap Scroll Indicator

Toggles the display of a side line showing which part of the buffer is currently displayed by the Minimap. The side line appear only if the Minimap height is bigger than the editor view height. `(default=true)`

![](https://github.com/atom-minimap/minimap/blob/master/resources/scroll-indicator.png?raw=true)

###### Plugins *

When plugins are installed, a setting is created for each to enable/disable them directly from the Minimap settings view.


###### Scroll Animation

Enable animations when scrolling the editor by clicking on the Minimap. `(default=false)`

###### Scroll Animation Duration

Duration of the scroll animation when clicking on the Minimap. `(default=300)`


###### Use Hardware Acceleration

If checked the Minimap scroll is done using a `translate3d` transform, otherwise the `translate` transform is used. `(default=true)`

###### Absolute Mode

When enabled the Minimap uses an absolute positioning, letting the editor's content flow below the Minimap. `(default=true)`

Note that this setting will do nothing if `Display Minimap On Left` is also enabled.

`false`|`true`
---|---
![](https://github.com/atom-minimap/minimap/blob/master/resources/normal-mode.png?raw=true)|![](https://github.com/atom-minimap/minimap/blob/master/resources/absolute-mode.png?raw=true)

##### Key Bindings

The Minimap package doesn't provide any default keybindings. But you can define your own as demonstrated below:

```coffee
'atom-workspace':
  'cmd-m': 'minimap:toggle'
  'ctrl-alt-cmd-j': 'minimap:generate-javascript-plugin'
  'ctrl-alt-cmd-b': 'minimap:generate-babel-plugin'
  'ctrl-alt-cmd-c': 'minimap:generate-coffee-plugin'
```

##### Tweaking The Minimap

###### Hiding scrollbars

If you want to hide the default editor scrollbar, edit your `style.less` (Open Your Stylesheet) and use the following snippet:

```css
atom-text-editor .vertical-scrollbar,
atom-text-editor::shadow .vertical-scrollbar {
  opacity: 0;
  width: 0;
}
```

###### Changing the Minimap's background

![minimap-custom-background](https://github.com/atom-minimap/minimap/blob/master/resources/minimap-custom-background.png?raw=true)

```css
atom-text-editor atom-text-editor-minimap,
atom-text-editor::shadow atom-text-editor-minimap {
  background: green;
}
```

###### Changing the color of the Minimap's `visible-area`

![minimap-custom-background](https://github.com/atom-minimap/minimap/blob/master/resources/minimap-custom-visible-area.png?raw=true)

```css
atom-text-editor atom-text-editor-minimap::shadow .minimap-visible-area,
atom-text-editor::shadow atom-text-editor-minimap::shadow .minimap-visible-area {
  background-color: green;
  opacity: .5;
}
```

###### Changing the color of the Minimap's `scroll-indicator`

![minimap-custom-background](https://github.com/atom-minimap/minimap/blob/master/resources/minimap-custom-scroll-indicator.png?raw=true)

```css
atom-text-editor atom-text-editor-minimap::shadow .minimap-scroll-indicator,
atom-text-editor::shadow atom-text-editor-minimap::shadow .minimap-scroll-indicator {
  background-color: green;
}
```

###### Disabling mouse interactions when in absolute mode

If you want to prevent to catch the mouse pointer when the `absoluteMode` setting is enabled you can use the following snippet to do so:

```css
atom-text-editor atom-text-editor-minimap,
atom-text-editor::shadow atom-text-editor-minimap {
  pointer-events: none;
}

atom-text-editor atom-text-editor-minimap::shadow .minimap-visible-area,
atom-text-editor::shadow atom-text-editor-minimap::shadow .minimap-visible-area {
  pointer-events: auto;
}
```

The visible area will still allow interaction but the Minimap track won't.

##### ASCII Art Comments

One neat trick is to use ASCII art to create huge comments visible in the minimap. This is really efficient when navigating huge files.

![ASCII Art Comments](https://github.com/atom-minimap/minimap/blob/master/resources/ascii-comments.png?raw=true)

To generate these comments you can use on these useful Atom packages:

- [Figlet](https://atom.io/packages/figlet)
- [Figletify](https://atom.io/packages/figletify)
- [Minimap Titles](https://atom.io/packages/minimap-titles)
- [Draw Package](https://atom.io/packages/draw-package)

----

#### Developers Documentation

You can find below the developers documentation on how to create Minimap's plugins and how to use decorations and stand-alone Minimaps.

For a more detailled documentation of the API make sure to check the [Minimap API Documentation](http://atom-minimap.github.io/minimap/).

##### Plugins

The Minimap comes with a plugin system used to extend the features displayed in it. Minimap plugins, once activated, are known and can be managed through the Minimap settings.

###### Plugin Generation Command

Use the `Generate Javascript Plugin`, `Generate Coffee Plugin` or `Generate Babel Plugin` commands, available in the command palette, to generate a new Minimap plugin package.

- `Minimap: Generate Javascript Plugin`: Will generate a vanilla JavaScript package.
- `Minimap: Generate Coffee Plugin`: Will generate a CoffeeScript package.
- `Minimap: Generate Babel Plugin`: Will generate a ES6 package that uses babel-js.

###### Plugins Controls

When the `displayPluginsControls` setting is toggled on, plugins activation can be managed directly from the Minimap package settings or by using the quick settings dropdown available on the Mimimap itself:

![Minimap Screenshot](https://github.com/atom-minimap/minimap/blob/master/resources/plugins-list.gif?raw=true)

##### Stand-alone Mode

Starting with version 4.13, the Minimap can operate in a stand-alone mode. Basically, it means that a Minimap can be appended to the DOM outside of a `TextEditor` and without being affected by it.

The example below demonstrates how to retrieve and display a stand-alone Minimap:

```js
atom.packages.serviceHub.consume('minimap', '1.0.0', (api) => {
  editor = atom.workspace.getActiveTextEditor()
  minimap = api.standAloneMinimapForEditor(editor)

  minimapElement = atom.views.getView(minimap)
  minimapElement.attach(document.body)
  minimapElement.style.cssText = `
    width: 300px;
    height: 300px;
    position: fixed;
    top: 0;
    right: 100px;
    z-index: 10;
  `
})
```

In a nutshell, here's the main changes to expect when using a stand-alone Minimap:

- In stand-alone mode, it's the `MinimapElement` that is responsible to sets the size of the underlying `Minimap` model, so you can give it any size and the Minimap will just adapt to it.
- Scrolling in the target `TextEditor` won't change the Minimap display.
- The mouse controls in the Minimap are removed.
- The visible area and the quick settings button are removed.
- Stand-alone Minimaps aren't dispatched in the `observeMinimaps` callback, so they won't be targeted by plugins and won't receive the decorations that plugins normally creates on Minimaps.

For the moment, stand-alone Minimaps still need a target `TextEditor` but I hope to make it work with just a path at some point.

##### Minimap Decorations

The Minimap package mimic the decoration API available on editors so that you can easily add your own decorations on the Minimap.

While the interface is the same, some details such as the available decorations types change relatively to the editor's decorations API.

###### Scope And Styling

The most important change is that decorations on the Minimap doesn't use a `class`, but rather a `scope`

```js
minimapView.decorateMarker(marker, {type: 'line', scope: '.scope .to .the.marker.style'})
```

It's still possible to pass a class parameter to the decoration:


```js
minimapView.decorateMarker(marker, {type: 'line', class: 'the marker style'})
```

In that case, when rendering the decoration a scope will be build that will look like `.minimap .editor .the.marker.style`.

The reason of using a scope rather than a class is that while editor's decorations are part of the DOM and benefit of the styles cascading, Minimap's decorations, rendered in a canvas, do not. In order to work around that, decoration's styles are defined using a `scope` property containing the selector allowing to retrieve the decoration style.

This allow the Minimap decorations to still be styled using css. For instance, the scope used by the `minimap-selection` package is:

```css
.minimap .editor .selection .region {
  /* ... */
}
```

Note that the scope is prefixed with `.minimap` so that you can override the selection style in the Minimap without impacting the editor's one.

Also note that only the `background` property will be retrieved to style a decoration.

A last option is to pass a css color directly in a `color` option, such as:

```js
minimapView.decorateMarker(marker, {type: 'line', color: '###ff0000'})
```

In that case neither the scope nor the class will be used.

###### Decorations Types

Another non-trivial change is the list of available decoration's type. At the time, the available types on the Minimap are:

- `line`: Same as the editor one, it colors the line background with a color extracted from the decoration scope.
- `highlight-under`: Correspond to an editor `highlight` decoration that is rendered before rendering the line content.
- `highlight-over`, `highlight`: Correspond to an editor `highlight` decoration that is rendered after having rendered the line content.
- `highlight-outline`: Correspond to an editor `highlight` decoration that is rendered only as an outline in the Minimap.

##### License

[MIT](./LICENSE)
##<a name="minimap-autohide"></a>[minimap-autohide](https://github.com/jayk/minimap-autohide#readme) 

Automatically hide the minimap when you aren't using it.

### minimap-autohide package

#### Hide your minimap until you need it.

This package automatically hides the minimap until you need it.

When editing normally, you have the entire window for your editor. As soon as you begin to scroll, the minimap appears and you can interact with it normally.

Written by @JayKuri - If you like it, say Hi!

![Minimap autohide animated image](https://raw.githubusercontent.com/jayk/minimap-autohide/master/screenshot.gif)

By default the minimap will be hidden when not scrolling, and will slide out from the right when scrolling.  You can, however, tweak the appearance. When you are scrolling, the minimap will have a class 'scrolling' added to it. You can therefore override the default by adding an entry to your personal styles.less file.

For example, this style entry restores the original look of the minimap, but causes the minimap to instantly disappear when not scrolling... for a more 'snap-in' effect.

    atom-text-editor::shadow {
      atom-text-editor-minimap.scrolling {
        left: 0px;
        display: block;
      }
      atom-text-editor-minimap {
        background: rgba(0,0,0,0.2);
        position: relative;
        display: none;
        left: 0px;
        opacity: 1;
      }
    }

Likewise, if you don't like the semi-transparent background, you can override it in your theme:

    atom-text-editor-minimap {
      // give us a nice dark-blue background
      background: ###000040;
    }

Known issues: Does not interact well with 'minimap-on-left' setting. You may, however, be able to set a style in your own styles.less that would allow it to work.
##<a name="minimap-bookmarks"></a>[minimap-bookmarks](https://github.com/atom-minimap/minimap-bookmarks#readme) 

Displays Atom bookmarks in the minimap

### minimap-bookmarks package [![Build Status](https://travis-ci.org/atom-minimap/minimap-bookmarks.svg?branch=master)](https://travis-ci.org/atom-minimap/minimap-bookmarks)

Displays Atom bookmarks in the minimap.

![Minimap Bookmarks Screenshot](https://github.com/atom-minimap/minimap-bookmarks/blob/master/screenshot.gif?raw=true)
##<a name="minimap-find-and-replace"></a>[minimap-find-and-replace](https://github.com/atom-minimap/minimap-find-and-replace#readme) 

Minimap bindings for the find and replace package

### minimap-find-and-replace package

Displays the search matches in the minimap.

![Minimap Screenshot](https://github.com/atom-minimap/minimap-find-and-replace/blob/master/screenshot.png?raw=true)

You will need the [Minimap package](https://github.com/atom-minimap/minimap) installed to use this package.
##<a name="minimap-git-diff"></a>[minimap-git-diff](https://github.com/atom-minimap/minimap-git-diff#readme) 

A minimap binding for the git diff package

### minimap-git-diff package

A minimap binding for the Atom git-diff package.

![Minimap Git Diff Screenshot](https://github.com/atom-minimap/minimap-git-diff/blob/master/screenshot.png?raw=true)

You will need the [Minimap package](https://github.com/fundon/atom-minimap) installed to use this package.
##<a name="minimap-hide"></a>[minimap-hide](https://github.com/T-800/atom-minimap-hide#readme) 

Hide the minimap when pane isn't focus

### minimap-hide package

####Hide the minimap when pane isn't focus

#### Installation
``` apm install minimap-hide ```

[![apm install {package}](http://tcyrus.me/apm/minimap-hide.svg?theme=solarized-dark)](https://atom.io/packages/minimap-hide)
##<a name="minimap-highlight-selected"></a>[minimap-highlight-selected](https://github.com/atom-minimap/minimap-highlight-selected#readme) 

A minimap binding for the highlight-selected package

### minimap-highlight-selected package

A minimap binding for the [highlight-selected package](https://github.com/richrace/highlight-selected).

![Screenshot](https://github.com/atom-minimap/minimap-highlight-selected/blob/master/screenshot.png?raw=true)

##### Customization

If you want to change the color of the minimap highlights use the following CSS rules in your user stylesheet:

```css
/* The rule for normal highlights */
.minimap .highlight-selected {
  background: blue;
}

/* The rule for selected highlights */
.minimap .highlight-selected.selected {
  background: red;
}
```
##<a name="minimap-linter"></a>[minimap-linter](https://github.com/nesukun/atom-minimap-linter#readme) 

Minimap bindings for atom-linter

### minimap-linter package

Atom package to display linter markers on minimap.

![minimap-linter](https://raw.githubusercontent.com/nesukun/atom-minimap-linter/master/minimap-linter.gif)
##<a name="minimap-pigments"></a>[minimap-pigments](https://github.com/abe33/minimap-pigments#readme) 

An Atom plugin to display pigments colors in the Minimap.

### minimap-pigments package [![Build Status](https://travis-ci.org/abe33/minimap-pigments.svg?branch=master)](https://travis-ci.org/abe33/minimap-pigments)

An Atom plugin to display pigments colors in the Minimap.

![Screenshot](https://github.com/abe33/minimap-pigments/blob/master/screenshot.png?raw=true)
##<a name="minimap-selection"></a>[minimap-selection](https://github.com/atom-minimap/minimap-selection#readme) 

Display the buffer's selections on the minimap

### minimap-selection package [![Build Status](https://travis-ci.org/atom-minimap/minimap-selection.svg?branch=v4.1.0)](https://travis-ci.org/atom-minimap/minimap-selection)

Display the buffer's selections on the minimap

![Screenshot](https://github.com/atom-minimap/minimap-selection/blob/master/screenshot.gif?raw=true)

#### Settings

##### Highlight Cursors Lines

When enabled, lines that holds a cursors will be highlighted in the minimap.

##### Customization

The selection color can be customized using the following CSS rule in your user stylesheet:

```css
.minimap-selection .region {
  background: green;
}
```

When the `Highlight Cursors Lines` setting is enabled the line's highlight color can be customized using the following CSS rule in your user stylesheet: 

```css
.minimap-selection .cursor-line {
  background: blue;
}
```
##<a name="npm-install"></a>[npm-install](https://github.com/hughsk/atom-npm-install#readme) 

Automatically install and save any missing npm modules being used in the current file

### npm-install [![stable](http://hughsk.github.io/stability-badges/dist/stable.svg)](http://github.com/hughsk/stability-badges) ###

[Atom](http://atom.io/) plugin to automatically install and save any selected
npm packages not already included in the closest `package.json` file.

![npm-install](http://i.imgur.com/i5FKsXH.gif)

#### Usage ####

1. Select the `require` or `import` statements of the
   packages you want to install.
2. Open the Command Palette, and type `npm install` to
   bring up the available commands.
3. Your packages will be installed. Enjoy!

#### Configuration Options

Accessible from `Settings > Packages > npm-install`:

* **Install Cache:** force your installations to always or never use the local cache.
* **Custom npm PATH lookup:** useful if you keep your npm
  in an unconventional location. Point this to the directory
  of your npm executable should you have
  [any issues](https://github.com/hughsk/atom-npm-install/issues/2).

#### Changelog

##### 3.0.0

* Packages must now be selected to be installed. This gives
  you control over which packages are being installed instead
  of trying to work that out for you, making it simpler to
  support [scoped packages](https://docs.npmjs.com/misc/scope) :sparkles:.
* The installation pane is now attached to the right
  instead of the bottom of the screen.
* ES6 support! No more parsing errors, also `import`
  statements can be installed like you would requires too.
* CoffeeScript is no longer supported. If you'd like that back, I'd recommend
sticking with the previous version or submitting a pull request to
[atom-selected-requires](https://github.com/hughsk/atom-selected-requires).

##### 2.0.0

As of version `2.0.0` keybindings are not included by default. If you miss
these shortcuts, simply add the following to your keymap file:

``` coffeescript
'.workspace':
  'ctrl-alt-i': 'npm-install:save'
  'ctrl-alt-d': 'npm-install:save-dev'
```

#### License ####

MIT. See [LICENSE.md](http://github.com/hughsk/npm-install/blob/master/LICENSE.md) for details.
##<a name="pane-layout-plus"></a>[pane-layout-plus](https://github.com/chemoish/atom-pane-layout#readme) 

Can has switch the layout of your panes.

### Atom.io – Pane Layout Package

Focus and control the layout of your atom editor.

#### Features

| Command | Mac | PC and Linux |
| --- | --- | --- |
| Set the column layout | Cmd + Alt + [1-5] | Alt + Shift + [1-5] |
|	Jump to column | Ctrl + [1-4] | Same |

#### Demo

![pane-layout](https://raw.github.com/chemoish/atom-pane-layout/master/demo.gif)

#### Nitty Gritty

 - When a layout is chosen that increases the pane count, any additional panes will be left empty.
 - When a layout is chosen that decreases the pane count, any left over panes will be collapsed into the last available pane.
 - When a layout is chosen and a custom layout is already in place, any left over panes will be collapsed into the last available pane.
 - When a layout is changed that causes panes to collapse, stay focused on the active file – iff the file is in the file system.
##<a name="pigments"></a>[pigments](https://github.com/abe33/atom-pigments#readme) 

A package to display colors in project and files.

[![Build Status](https://travis-ci.org/abe33/atom-pigments.svg?branch=master)](https://travis-ci.org/abe33/atom-pigments)

#### <img src='https://cdn.rawgit.com/abe33/atom-pigments/master/resources/logo.svg' width='320' height='80'>

A package to display colors in project and files:

![Screenshot](https://github.com/abe33/atom-pigments/blob/master/resources/pigments.gif?raw=true)

Pigments will scan source files in your project directories looking for colors and will build a palette with all of them. Then for each opened file, it will use the palette to evaluate the value of a given color. The legible source paths can be defined through various settings either at the global or per project level. **By default colors in every file will be highlighted, to limit the display of colors to the desired filetype only please see the [Defining Where Pigments Applies](###defining-where-pigments-applies) below.**

Pigments supports out of the box most of the color transformations functions and expressions of the three biggest CSS pre-processors out there, namely LESS, Sass and Stylus. However, it doesn't mean pigments is able to parse and understand all of these languages constructs. For the moment, Pigments' aim is to support the widest range of usage, even if it implies reducing its ability to parse certain complex constructs. You can refer to the [parser specs](https://github.com/abe33/atom-pigments/blob/master/spec/color-parser-spec.coffee) for an exhaustive list of the supported expressions.

#### Install

Using `apm`:

```
apm install pigments
```

Or search for `pigments` in Atom settings view.

#### Defining Where Pigments Applies

By default, Pigments will highlight every color in every file, but you can limit that using the two settings [`Supported Filetypes`](###supported-filetypes) and [`Ignored Scopes`](###ignored-scopes).

The first setting allow you to specify the list of extensions where pigments will apply. For instance, by using the values `css, less`, colors will be visible only in CSS and Less files.

The second setting takes an array of regular expression strings used to exclude colors in specific scopes (like comments or strings). You can find the scope that applies at the cursor position with the `Editor: Log Cursor Scope` command (<kbd>cmd-alt-p</kbd> or <kbd>ctrl-alt-shift-p</kbd>).

![get scope](https://github.com/abe33/atom-pigments/blob/master/resources/get-scope.gif?raw=true)

#### Defaults File

Pigments is able to follow variables uses up to a certain point, if a color refers to several variables whose values can't be evaluated (because they use unsupported language-specific features) the color will be flagged as invalid and not displayed. This can be problematic when it happens on the core components of a complex palette.

To solve that issue, you can define a *defaults file* named `.pigments` at the root of a project directory and you can put in it all the variables declarations to use if a value from the sources files can't be evaluated.

This can also be used when your project core palette is dynamically defined so that pigments can evaluate properly the rest of the project colors.

#### Commands

**Note:** Pigments doesn't define any keybindings for the provided commands, instead it'll let you define your own keybindings.

##### Pigments: Show Palette

You can display the project's palette through the `Pigments: Show Palette` command from the command palette:

![Screenshot](https://github.com/abe33/atom-pigments/blob/master/resources/palette.gif?raw=true)

The project palette is made of all the colors that are affected to a variable, which means it won't display hardcoded colors affected to a CSS property. If you want to find every color used in a project, including the hardcoded colors in CSS files, use the `Pigments: Find Colors` instead.

Patterns for Less, Sass, Scss and Stylus variables are currently supported, which includes:

```stylus
my-var = ###123456 // stylus
```
```sass
$my-var: ###123456 // sass
$my-var: ###123456; // scss
```
```css
@my-var: ###123456; /* less */
```

As with every command, this command can be triggered using the keyboard by defining a keybinding like this:

```coffee
'atom-workspace':
  'alt-shift-p': 'pigments:show-palette'
```

##### Pigments: Find Colors

You can search for all colors in your project using the `Pigments: Find Colors` command from the command palette:

![Screenshot](https://github.com/abe33/atom-pigments/blob/master/resources/search.gif?raw=true)

The results will include colors declared in variables, places where the color variables are used as well as hardcoded color values in every file that matches one of the patterns defined in both `pigments.sourceNames` and `pigments.extendedSearchNames` settings.

By default this includes:

```
**/*.css
**/*.less
**/*.scss
**/*.sass
**/*.styl
**/*.stylus
```

This command can be triggered using the keyboard by defining a keybinding like this:

```coffee
'atom-workspace':
  'alt-shift-f': 'pigments:find-colors'
```

##### Pigments: Convert To Hexadecimal/Pigments: Convert to RGB(A)

It evaluates and replace a color by either its hexadecimal notation or rgb/rgba notation.
Accessible from the command palette or by right clicking on a color.

![pigments-conversion](https://github.com/abe33/atom-pigments/blob/master/resources/context-menu-conversion.gif?raw=true)

These commands can be triggered using the keyboard by defining a keybinding like this:

```coffee
'atom-workspace':
  'alt-shift-h': 'pigments:convert-to-hex'
  'alt-shift-g': 'pigments:convert-to-rgb'
  'alt-shift-j': 'pigments:convert-to-rgba'
```

When triggered from the command palette or from the keyboard, the conversion will operate on every cursor positioned on color markers.

##### Pigments: Project Settings

Each Pigments project has its own set of settings that can extend or replace the global configuration. These settings are available through the `pigments:project-settings` command:

![pigments-conversion](https://github.com/abe33/atom-pigments/blob/master/resources/project-settings.png?raw=true)

The `Source Names`, `Ignored Names`, `Ignored Scopes` and `Extended Search Names` fields all match a global configuration. When defined the project will use both the global config and the one of the current project, except when the `Ignore Global` checkbox is checked.

The `Include Atom Themes Stylesheets` setting is specific to the project and can't be defined globally. When enabled, it'll add all the public themes variables in the current project palette:

![pigments-conversion](https://github.com/abe33/atom-pigments/blob/master/resources/project-settings.gif?raw=true)

**Note that it won't add all the variables defined in the less files of the syntax and ui themes, only the ones that must be present as defined in the [themes documentation](https://atom.io/docs/latest/hacking-atom-creating-a-theme).**

**This feature is still quite experimental at this stage.**

##### Pigments: Reload

This command will force a reload of all variables in the project, this can be useful when the serialized state of the plugin contains invalid data and you want to get rid of them without having to touch to the content of the `.atom/storage` directory.

This command can be triggered using the keyboard by defining a keybinding like this:

```coffee
'atom-workspace':
  'alt-shift-r': 'pigments:reload'
```

#### Settings

##### Source Names

An array of glob patterns of the files to use as source for the project's variables and colors.

* Key: `pigments.sourceNames`
* Default: `['**/*.styl', '**/*.stylus', '**/*.less', '**/*.sass', '**/*.scss']`

##### Ignored Names

An array of glob patterns of the files to ignore as source files for the project's variables and colors.

* Key: `pigments.ignoredNames`
* Default: `['node_modules/*']`

##### Extended Search Names

An array of glob patterns of files to include in the `Pigments: Find Colors` scanning process.

* Key: `pigments.extendedSearchNames`
* Default: `['**/*.css']`

##### Supported Filetypes

An array of file extensions where colors will be highlighted. If the wildcard `*` is present in this array then colors in every file will be highlighted.

* Key: `pigments.supportedFiletypes`
* Default: `['*']`

##### Ignored Scopes

An array of regular expressions strings to match scopes to ignore when rendering colors in a text editor.

For instance, if you want to ignore colors in comments and strings in your source files, use the following value:

```
\.comment, \.string
```

As you can notice, the `.` character in scopes are escaped. This is due to the fact that this setting uses javascript `RegExp` to test the token's scope and the `.` is used to match against any character.

For instance, to ignores colors in html attributes you can use the following expression:

```
\.text\.html(.*)\.string
```

Note the `(.*)` in the middle of the expression. It'll ensure that we're searching for the `.string` scope in the `.text.html` grammar even if there's other scope between them by catching any character between the two classnames.

To find which scope is applied at a given position in a buffer you can use the `editor:log-cursor-scope` command. From that you'll be able to determine what expression to use to match the scope.

* Key: `pigments.ignoredScopes`
* Default: `[]`

##### Autocomplete Scopes

The autocomplete provider will only complete color names in editors whose scope is present in this list.

* Key: `pigments.autocompleteScopes`
* Default: `['.source.css', '.source.css.less', '.source.sass', '.source.css.scss', '.source.stylus']`

##### Extend Autocomplete To Variables

When enabled, the autocomplete provider will also provides completion for non-color variables.

* Key: `pigments.extendAutocompleteToVariables`
* Default: `false`

##### Traverse Into Symlink Directories

Whether to traverse symlinked directories to find source files or not.

* Key: `pigments.traverseIntoSymlinkDirectories`
* Default: `false`

##### Ignore VCS Ignored Paths

When this setting is enabled, every file that are ignored by the VCS will also be ignored in Pigments. That means they'll be excluded when searching for colors and when building the project palette.

* Key: `pigments.ignoreVcsIgnoredPaths`
* Default: `true`

##### Marker Type

Defines the render mode of color markers. The possible values are:

<table>
  <tr>
    <th>background</th>
    <th>outline</th>
    <th>underline</th>
  </tr>
  <tr>
    <td>
      <img src='https://github.com/abe33/atom-pigments/blob/master/resources/background-renderer.png?raw=true'/>
    </td>
    <td>
      <img src='https://github.com/abe33/atom-pigments/blob/master/resources/outline-renderer.png?raw=true'/>
    </td>
    <td>
      <img src='https://github.com/abe33/atom-pigments/blob/master/resources/underline-renderer.png?raw=true'/>
    </td>
  </tr>
  <tr>
    <th>dot</th>
    <th>square-dot</th>
    <th>gutter</th>
  </tr>
  <tr>
    <td>
      <img src='https://github.com/abe33/atom-pigments/blob/master/resources/dot-renderer.png?raw=true'/>
    </td>
    <td>
      <img src='https://github.com/abe33/atom-pigments/blob/master/resources/square-dot-renderer.png?raw=true'/>
    </td>
    <td>
      <img src='https://github.com/abe33/atom-pigments/blob/master/resources/gutter-color.png?raw=true'/>
    </td>
  </tr>
</table>

* Key: `pigments.markerType`
* Default: `'background'`

##### Sort Palette Colors

The type of sorting applied to the colors in the palette view. It can be changed directly from the palette view.

* Key: `pigments.sortPaletteColors`
* Default: `'none'`

##### Group Palette Colors

Defines how the colors are grouped together in the palette view. It can be changed directly from the palette view.

* Key: `pigments.groupPaletteColors`
* Default: `'none'`

##### Merge Duplicates

Defines whether to merge colors duplicates together as a single result in the palette view. It can be changed directly from the palette view.

* Key: `pigments.mergeDuplicates`
* Default: `false`

##### Delay Before Scan

Pigments rescans the text buffer once you stopped editing it, however as the process can be sometime expensive, it'll apply an extra delay after the dispatch of the `did-stop-changing` event before starting the scanning process. This setting define the number of milliseconds to wait after the `did-stop-changing` event before starting to scan the buffer again. If your start typing in the buffer again in this interval, the rescan process will be aborted.

* Key: `pigments.delayBeforeScan`
* Default: `500` (ms)
##<a name="react-snippets"></a>[react-snippets](https://github.com/webbushka/atom-react-snippets) 

Atom Snippets for React, React Router and Flux

Atom React.js Snippets [![Build Status](https://travis-ci.org/webbushka/atom-react-snippets.svg?branch=master)](https://travis-ci.org/webbushka/atom-react-snippets)
====================================================================================================================================================================

An [Atom](https://atom.io/) snippet library for React, React Router and Flux. This library uses ES6 syntax, if you would prefer ES5 or Coffeescript snippets please use the [Atom React Package](https://atom.io/packages/react).

Install
-------

Go to `Packages > Settings View > Open` once in settings go to the Install tab and search for **react-snippets**

Development
-----------

```sh
$ cd ~/.atom/packages
$ git clone https://github.com/webbushka/atom-react-snippets.git
$ cd atom-react-snippets
$ apm install
$ apm link
```

Features
--------

-	React Snippets
-	React Router Snippets - Needs update from v0.13 to v1.0
-	Flux Snippets

Contributing
------------

1.	Fork it!
2.	Create your feature branch: `git checkout -b my-new-feature`
3.	Commit your changes: `git commit -m 'Add some feature'`
4.	Push to the branch: `git push origin my-new-feature`
5.	Submit a pull request

Change Log
----------

[It's over here!](https://github.com/webbushka/atom-react-snippets/wiki/Changelogs)

License
-------

[MIT License](http://zenorocha.mit-license.org/) © Zeno Rocha

Credit
------

The React.js snippets were originally created by [orktes](https://atom.io/users/orktes) in [Atom React](https://atom.io/packages/react) in ES5 syntax.
##<a name="regex-railroad-diagram"></a>[regex-railroad-diagram](https://github.com/klorenz/atom-regex-railroad-diagrams#readme) 

Display railroad diagram of regex under cursor.

### regex-railroad-diagram package

A regular expression railroad diagram view for regular expression 
under cursor.  This is still in development and for me it is a test of
graphics capabilities of Atom.

![regex-railraod-diagram in action](https://raw.githubusercontent.com/klorenz/atom-regex-railroad-diagrams/3552667228c192e81a0d2e5843e824c064b8e4b9/regex-railroad-diagrams.png)

It also shows you a parsing error message, if your regex is not syntactically
correct.

For now it only supports most common regex features, but there are more 
to come.

##<a name="regex-tester"></a>[regex-tester](https://github.com/deprint/regex-tester#readme) 

Test Javascript regular expressions

regex-tester
============
[![Build Status](https://travis-ci.org/deprint/regex-tester.svg)](https://travis-ci.org/deprint/regex-tester) [![Dependency Status](https://david-dm.org/deprint/regex-tester.svg)](https://david-dm.org/deprint/regex-tester) [![apm](https://img.shields.io/apm/dm/regex-tester.svg)](https://github.com/deprint/regex-tester) [![apm](https://img.shields.io/apm/v/regex-tester.svg)](https://github.com/deprint/regex-tester)

#### Test Javascript regular expressions
![regex](https://cloud.githubusercontent.com/assets/7817714/8729643/9f46654c-2bec-11e5-8edd-5f026ca45391.png)

Run `regex-tester:toggle` to open the panel
##<a name="sort-lines"></a>[sort-lines](https://github.com/atom/sort-lines#readme) 

Sorts your lines. Never gets tired.

### Sort Lines Package [![Build Status](https://travis-ci.org/atom/sort-lines.svg?branch=master)](https://travis-ci.org/atom/sort-lines)

Sorts your lines in Atom, never gets tired.

![sort-lines-demo](https://f.cloud.github.com/assets/2988/1796891/85e69ff2-6a93-11e3-89ac-31927f604592.gif)
##<a name="terminal-plus"></a>[terminal-plus](https://atom.io/packages/terminal-plus) 

A terminal package for Atom, complete with themes and more.

#### Author's Note
* Please make sure you are on the [latest version of Atom](https://atom.io/releases) before reporting bugs!
* This package requires that you have the dependencies for node-gyp.  
[See node-gyp install instructions](https://github.com/nodejs/node-gyp###installation).  
* You must use a monospaced font in order for the spacing to be right.
* Having issues on Windows 10? [Try this](https://github.com/jeremyramin/terminal-plus/issues/15###issuecomment-144618245).

### Terminal-Plus
Terminal-Plus is a terminal package for Atom, complete with themes and more.  

![demo](https://github.com/jeremyramin/terminal-plus/raw/master/resources/demo.gif)

*[Nucleus Dark UI](https://atom.io/themes/nucleus-dark-ui) with [Atom Material Syntax](https://atom.io/themes/atom-material-syntax) and our Homebrew theme.*

#### Usage
Terminal-Plus stays in the bottom of your editor while you work.

##### Status Bar
![status-bar](https://github.com/jeremyramin/terminal-plus/raw/master/resources/status-bar.png)  
You can keep track of terminal instances via the status bar. Each terminal has a status icon ( ![status icon](https://github.com/jeremyramin/terminal-plus/raw/master/resources/status-icon.png) ) in the status bar. The ( ![plus-icon](https://github.com/jeremyramin/terminal-plus/raw/master/resources/plus-icon.png) ) button creates a new terminal, while the ( ![red-x](https://github.com/jeremyramin/terminal-plus/raw/master/resources/red-x.png) ) button closes all terminals.

Click on a status icon to toggle that terminal. Right click the status icon for a list of available commands. From the right-click menu you can color code the status icon as well as hide or close the terminal instance.

##### Terminal
You can open the last active terminal with the `terminal-plus:toggle` command (Default:`` ctrl-` ``).  If no terminal instances are available, then a new one will be created. The same toggle command is used to hide the currently active terminal.

From there you can begin typing into the terminal. By default the terminal will change directory into the project folder if possible. The default working directory can be changed in the settings to the home directory or to the active file directory.

[See available commands below](###commands).

#### Features

##### Full Terminal
Every terminal is loaded with your system’s default initialization files. This ensures that you have access to the same commands and aliases as you would in your standard terminal.

##### Themes
The terminal is preloaded with several themes that you can choose from. Not satisfied?  
Use the following template in your stylesheet:
```css
.terminal-plus .xterm {
  background-color: ;
  color: ;

  ::selection {
    background-color: ;
  }

  .terminal-cursor {
    background-color: ;
  }
}
```

##### Process Titles
By hovering over the terminal status icon, you can see which command process is currently running in the terminal.

![](https://github.com/jeremyramin/terminal-plus/raw/master/resources/terminal_title.png)

##### Terminal Naming
Need a faster way to figure out which terminal is which? Name your status icons!

![](https://github.com/jeremyramin/terminal-plus/raw/master/resources/status-icon_rename.png)

Available via the status icon context menu.

![](https://github.com/jeremyramin/terminal-plus/raw/master/resources/status-icon_rename-dialog.png)

##### Color Coding
Color code your status icons!

![](https://github.com/jeremyramin/terminal-plus/raw/master/resources/status-icon_color_coding.png)

The colors are customizable in the settings, however the color names remain the same in the context menu.

##### Sorting
Organize your open terminal instances by dragging and dropping them.

![](https://github.com/jeremyramin/terminal-plus/raw/master/resources/sorting.gif)

##### Resizable
You can resize the view vertically, or just maximize it with the maximize button.

##### Working Directory
You can set the default working directory for new terminals. By default this will be the project folder.

##### File Dropping
Dropping a file on the terminal will insert the file path into the input. This works with external files, tabs from the Atom tab-view, and entries from the Atom tree-view.

##### Insert Selected Text
Insert and run selected text from your text editor by running the `terminal-plus:insert-selected-text` command (`ctrl-enter`).

![](https://github.com/jeremyramin/terminal-plus/raw/master/resources/insert_selected_text.gif)

If you have text selected, it will insert your selected text into the active terminal and run it.  
If you don't have text selected it, will run the text on the line where your cursor is then proceed to the next line.

##### Quick Command Insert
Quickly insert a command to your active terminal by executing the `terminal-plus:insert-text` command.

![](https://github.com/jeremyramin/terminal-plus/raw/master/resources/insert_text.png)

A dialog will pop up asking for the input to insert. If you have the `Run Inserted Text` option enabled in the settings (default is false), Terminal-Plus will automatically run the command for you.

###### Support for Special Keys
Support for IME, dead keys and other key combinations via the `Insert Text` dialog box. Just click the keyboard button in the top left of the terminal or set up a keymap to the `terminal-plus:insert-text` command.

![](https://github.com/jeremyramin/terminal-plus/raw/master/resources/special_keys.gif)

Note: Make sure you have the `Run Inserted Command` toggle off otherwise it will run your inserted text.

##### Map Terminal To
Map your terminals to each file or folder you are working on for automatic terminal switching.

###### File
![](https://github.com/jeremyramin/terminal-plus/raw/master/resources/map_terminals_to_file.gif)

###### Folder
![](https://github.com/jeremyramin/terminal-plus/raw/master/resources/map_terminals_to_folder.gif)

Toggling the `Auto Open a New Terminal (For Terminal Mapping)` option will have the mapping create a new terminal automatically for files and folders that don't have a terminal. The toggle is located right under the `Map Terminals To` option.

![](https://github.com/jeremyramin/terminal-plus/raw/master/resources/map_terminals_to_auto_open.gif)

#### Install
Ready to install?

You can install via apm: `apm install terminal-plus`

Or navigate to the install tab in Atom’s settings view, and search for `terminal-plus`.

#### Commands
| Command | Action | Default Keybind |
|---------|--------|:-----------------:|
| terminal-plus:new | Create a new terminal instance. | `ctrl-shift-t`<br>or<br>`cmd-shift-t` |
| terminal-plus:toggle | Toggle the last active terminal instance.<br>**Note:** This will create a new terminal if it needs to. | `` ctrl-` ``<br>(Control + Backtick) |
| terminal-plus:prev | Switch to the terminal left of the last active terminal. | `ctrl-shift-j`<br>or<br>`cmd-shift-j` |
| terminal-plus:next | Switch to the terminal right of the last active terminal. | `ctrl-shift-k`<br>or<br>`cmd-shift-k` |
| terminal-plus:insert-selected-text | Run the selected text as a command in the active terminal. | `ctrl-enter` |
| terminal-plus:insert-text | Bring up an input box for using IME and special keys. | –––––––––––– |
| terminal-plus:close | Close the active terminal. | `ctrl-shift-x`<br>or<br>`cmd-shift-x` |
| terminal-plus:close-all | Close all terminals. | –––––––––––– |
| terminal-plus:rename | Rename the active terminal. | –––––––––––– |

#### To-Do List
- [ ] Possibly merge dependencies into Terminal-Plus?
- [ ] Add support for dead keys and IME input
- [x] Add support for terminal tabs
- [x] Add support for automatic directory switching
- [x] Fix Atom requesting a rebuild after every update
- [x] Update winpty in pty.js dependency
- [x] Add support for custom ANSI colors in terminal
- [x] Fix `ctrl+c` for bash prompts on OS X and Linux
- [x] Add support for status icon names
##<a name="tomorrow-night-eighties-syntax"></a>[tomorrow-night-eighties-syntax](https://github.com/rockymadden/tomorrow-night-eighties-syntax-theme#readme) 

Tomorrow Night Eighties syntax theme for Atom.

### Tomorrow Night Eighties Atom Syntax Theme

Atom syntax theme using the ever popular Tomorrow Night Eighties colors:

![](https://github.com/ChrisKempson/Tomorrow-Theme/raw/master/Images/Tomorrow-Night-Eighties-Palette.png)
