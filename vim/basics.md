`f<a character> or t` navigates by `;` and `,`
`F<a character> or T` navigates by `;` and `,`
`#` and `*`

### Rules

1. Operator + Motion
2. When the same operator is used twice continuously, it will apply on current line. (`dd`, `>>`, `gUgU` or `gUU`)


## Normal mode
### Operator
| Operator | Description        | Tips   |
| -------- | ------------------ | ------ |
| `c`      | Change             | `C == c$`, `c<Number>w` instead of `d<Number>wa` |
| `d`      | Delete             | Delete a word: `daw` (Including a blank), Delete a paragraph: `dap` |
| `y`      | Copy to register   |
| `g~`     | Flip case          |
| `gu`     | To lowercase       | `guaw` |
| `gU`     | To uppercase       | `gUap` |
| `>`      | Add indentation    |
| `<`      | Reduce indentation |
| `=`      | Auto indentation   |
Others: `!, gq, g?, zf, g@`

Custom operator: `:h:map-operator`. e.g. `\\` in *commentary.vim* for comment.

### Motion
`h, j, k, l, /, ?, w, e, b`
`it`: between tags
e.g. `2?the`
`/pattern<CR>` and `?pattern<CR>`

Custom motion: `:h omap-info`. e.g. `ae` in `textobj-entire` as the entire file.


### Operator-Pending mode
It's activated after operator is hit, waiting for motion. The mode between hits `d` and `w`.


## Insert mode

用好`<Esc>`: 因为vim按块撤销，因此有时候可用**`<Esc>o`**代替`<CR>`，这样在撤销时更有粒度。
另，在插入模式中使用`<Up>, <Down>, <Left>, <Right>`时会产生一个新的撤销块。

| Operation   | Description                           |
| ----------- | ------------------------------------- |
| \<C-h\>     | Delete                                |
| \<C-w\>     | Delete last word                      |
| **\<C-u\>** | Delete till the beginning of the line |

- Back to normal mode
  - `<Esc>` or `<C-[>`
  - Insert-normal mode `<C-o>`
    - A special normal mode. It will change to insert mode after one command.
    - Tip: `<C-o>zz` - Put current line to the middle of screen
- Register
  - copy and paste
    - `yt{char}` copy contents till `{char}` to register
    - `<C-r>{register}` paste what's in `{register}` as typed from keyboard
      - `<CR>` or indentation may apply
    - or use `<C-r><C-p>{register}` to paste as original format
  - Calculation
    - "6 chairs, each costing \$35, totals \$\$"
    - `<C-r>=6*35<CR>`
- Insert arbitary code
  - `<C-v>{code}` and `<C-k>{code1}{code2}`
    - e.g. `<C-v>065`, `<C-v>u00bf`
    - e.g. `<C-k><<`, `<C-k>13`, `<C-k>?|`

## Visual Mode
| Command            | Description                       |
| ------------------ | --------------------------------- |
| `v`                | character                         |
| `V`                | line                              |
| `<C-v>`            | block                             |
| `gv`               | reselect last high lighted area   |
| `<Esc>` or `<C-[>` | back to normal mode               |
| `o` toggle active end of high lighted area             |

`b`, `e` is still usable in Visual mode

## Command Line Mode
Vim provides Ex commands for almost all functions. Get the full list by `:h ex-cmd-index`.
Ex commands are power to process multiple lines at once without moving the cursor.
Enter by `:`.

| Comman                                        | Description |
| --------------------------------------------- | ----------- |
| :[range]delete [x]                            | delete what's in range [to the register x]    |
| :[range]yank [x]                              | copy what's in range [to the register x]      |
| :[line]put [x]                                | paste what's in the register x after the line |
| :[range]copy {address}                        | copy what in range to address                 |
| :[range]move {address}                        | move what in range to address                 |
| :[range]join                                  | join what's in range                          |
| :[range]normal {commands}                     | excecute normal mode command {commands} to every line of the range |
| :[range]substitute/{pattern}/{string}/[flags] | Replace all matched {pattern} in the range with {string}           |
| :[range]global/{pattern}/[cmd]                | Execute {cmd} on all matched {pattern} in the range                |


### `[range]`
