# Vim

### Basic Commands
* vim filename: Open a file in Vim
* :q: Quit Vim
* :w: Save changes
* :wq or :x: Save and quit
* :q!: Quit without saving changes

### Navigation
* h, j, k, l: Move left, down, up, right
* w: Move to next word
* b: Move to previous word
* 0: Move to beginning of line
* $: Move to end of line
* gg: Go to first line of document
* G: Go to last line of document

### Editing
* i: Enter insert mode before cursor
* a: Enter insert mode after cursor
* o: Open a new line below and enter insert mode
* O: Open a new line above and enter insert mode
* x: Delete character under cursor
* dd: Delete entire line
* yy: Copy entire line
* p: Paste after cursor
* P: Paste before cursor

### Search and Replace
* /pattern: Search forward for pattern
* ?pattern: Search backward for pattern
* n: Repeat search in same direction
* N: Repeat search in opposite direction
* :%s/old/new/g: Replace all occurrences of 'old' with 'new' in the file

### Visual Mode
* v: Enter visual mode
* V: Enter visual line mode
* Ctrl+v: Enter visual block mode

### Multiple Files
* :e filename: Open a file in a new buffer
* :bn: Go to next buffer
* :bp: Go to previous buffer
* :bd: Close current buffer

### Split Windows
* :split filename: Open a file in a horizontal split
* :vsplit filename: Open a file in a vertical split
* Ctrl+w + h/j/k/l: Navigate between splits

### Macros
* qa: Start recording a macro named 'a'
* q: Stop recording macro
* @a: Play macro 'a'

### Miscellaneous
* u: Undo
* Ctrl+r: Redo
* .: Repeat last command
* :set number: Show line numbers
* :set nonumber: Hide line numbers
