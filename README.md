
This is an experimental tree-based writing interface for GPT-3. The code is actively being developed and thus 
unstable and poorly documented.

# Features

* Read mode
   * Linear story view
   * Tree nav bar
   * Edit mode
   
   
* Tree view
   * Explore tree visually with mouse
   * Expand and collapse nodes
   * Change tree topology
   * Edit nodes in place
   
   
* Navigation
   * Hotkeys
   * Bookmarks
   * Chapters
   * 'Visited' state   
   

* Generation
   * Generate N children with GPT-3
   * Modify generation settings 
   * Change hidden memory on a node-by-node basis
   

* File I/O
   * Open/save trees as JSON files 
   * Work with trees in multiple tabs
   * Combine trees
   

# Demo

![](static/readme/read-view.png)
![](static/readme/read-view-light.png)
![](static/readme/tree-view.png)
![](static/readme/tree-view-light.png)
![](static/readme/metadata-light.png)

ooo what features! wow so cool

# Hotkeys

*Alt hotkeys correspond to Command on Mac*

### File

Open: `o`, `Control-o`

Import JSON as subtree: `Control-Shift-O`

Save: `s`, `Control-s`


### Dialogs

Change chapter: `Control-y`

Preferences: `Control-p`

Generation Settings: `Control-Shift-P`

Visualization Settings: `Control-u`

Multimedia dialog: `u`

Tree Info: `Control-i`

Node Metadata: `Control+Shift+N`

Run Code: `Control+Shift+B`


### Mode / display

Toggle edit / save edits: `e`, `Control-e`

Toggle story textbox editable: `Control-Shift-e`

Toggle visualize: `j`, `Control-j`

Toggle bottom pane: `Tab`

Toggle side pane: `Alt-p`

Toggle show children: `Alt-c`

Hoist: `Alt-h`

Unhoist: `Alt-Shift-h`


### Navigate

Click to go to node: `Control-shift-click`

Next: `period`, `Return`, `Control-period`

Prev: `comma`, `Control-comma`

Go to child: `Right`, `Control-Right`

Go to next sibling: `Down`, `Control-Down`

Go to parent: `Left`, `Control-Left`

Go to previous Sibling: `Up`, `Control-Up`

Return to root: `r`, `Control-r`

Walk: `w`, `Control-w`

Go to checkpoint: `t`

Save checkpoint: `Control-t`

Go to next bookmark: `d`, `Control-d`

Go to prev bookmark: `a`, `Control-a`

Search ancestry: `Control-f`

Search tree: `Control-shift-f`

Click to split node: `Control-alt-click`

Goto node by id: `Control-shift-g`


### Organization 

Toggle bookmark: `b`, `Control-b`

Toggle archive node: `!`



### Generation and memory

Generate: `g`, `Control-g`

Inline generate: `Alt-i`

Add memory: `Control-m`

View current AI memory: `Control-Shift-m`

View node memory: `Alt-m`


### Edit topology

Delete: `BackSpace`, `Control-BackSpace`

Merge with Parent: `Shift-Left`

Merge with children: `Shift-Right`

Move node up: `Shift-Up`

Move node down: `Shift-Down`

Change parent: `Shift-P`

New root child: `Control-Shift-h`

New Child: `h`, `Control-h`, `Alt-Right`

New Parent: `Alt-Left`

New Sibling: `Alt-Down`



### Edit text

Toggle edit / save edits: `Control-e`

Save edits as new sibling: `Alt-e`

Click to edit history: `Control-click`

Click to select token: `Alt-click`

Next counterfactual token: `Alt-period`

Previous counterfactual token: `Alt-comma`

Apply counterfactual changes: `Alt-return`

Enter text: `Control-bar`

Escape textbox: `Escape`

Prepend newline: `n`, `Control-n`

Prepend space: `Control-Space`



### Collapse / expand

Collapse all except subtree: `Control-colon`

Collapse node: `Control-question`

Collapse subtree: `Control-minus`

Expand children: `Control-quotedbl`

Expand subtree: `Control-plus`


### View

Center view: `l`, `Control-l`

Reset zoom: `Control-0`



# Instructions

1. Install [direnv](https://github.com/direnv/direnv).

1. Use the `.envrc.sample` as a template for your `.envrc`.
   ```
   cp .envrc.sample .envrc
   ```

1. Add your API key to `.envrc`.

1. Install python 3.9 with [pyenv](https://github.com/pyenv/pyenv).

1. Set up venv in the project root.
   ```
   python -m venv venv
   ```

1. Activate venv.
   ```
   source venv/bin/activate
   ```

1. Install requirements.
   ```
   pip install -r requirements.txt
   ```

3. Run `main.py`.
   ```
   python main.py
   ```
4. Load a json tree.
5. Read :)
