# Notation
Vim keys combination can be represented in tree ways:
- `^v , Ctrl-v ,<C-v>` all represent ctlr+v
- `Shift-v ,<S-v>` all represent shift+v

# Modes
1. Normal Mode
2. Insert Mode - Opens up with i
3. Replace Mode - Opens with <S-r>
4. Visual Mode - Opens with v .
	1. Visual Line - Opens up with <S-v>
	2. Visual Block - Opens up with <C-v>
5. Command Mode - Opens with :

# Movement
1. To move top of page- H
2. To move to middle of page- M
3. To move to bottom of page- B
4. To move x line up or down- line-number+(j or k) // Relative Line Number in Vim.
5. To move to end of file- G
6. To move to start of file- gg
7. To move cursor ahead and back by one word - w and b
8. To move cursor to end of word - e
9. To move down and up with greater speed - <C-e> and <C-u>
10. To move cursor to highest , middle and lowest part of the visible screen - H , M and L
11. To move cursor on and before a character - f and t
12. Add text to one line below and above - o and <S-o>
13. To move to previous cursor postion - <C-o>

# Delete
1. To delete a character- x
2. To delete till a character- dt+(character)
3. To delete end of the word - de
4. To delete a line - dd
5. To delete x number of words - dxw
6. To delete up-to and including that character-df+(character) For more- [Meaning Of t and f](https-//stackoverflow.com/questions/12495442/what-do-the-f-and-t-commands-do-in-vim)

# Searching
1. To search a character- :/+(character)
2. To move ahead and backward through a list of search- n and `<S-n>`
3. To remove highlight from searched character- :noh
4. To search word under cursor- *
5. To search word under cursor in backward motion- #

# Modifiers
1. To change word inside a character - ci(ie inside)+(character)
2. To change word around a character - ca(ie around)+(character)

# Buffers
1. To split current buffer into half- :sp
2. To undo and redo change - u and <C-r>
3. To copy and paste - y and p
4. To paste above the current line - <S-p>

# Others
1. To open link in browser- gx
2. To move to given line number- line-number G // Without using relative line number

# Coc bindings
1. Spell Check Using Coc-Action-\(leader key)+w(for current word) For more- [Coc Spell Github](https-//github.com/iamcco/coc-actions)
