st - simple terminal
--------------------
st is a simple terminal emulator for X which sucks less.


Requirements
------------
In order to build st you need the Xlib header files.


Installation
------------
Edit config.mk to match your local setup (st is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install st (if
necessary as root):

    make clean install


Running st
----------
If you did not install st with make clean install, you must compile
the st terminfo entry with the following command:

    tic -sx st.info

See the man page for additional details.

Credits
-------
Based on Aurélien APTEL <aurelien dot aptel at gmail dot com> bt source code.

Patches
-------

- [Alpa focus highlight](https://st.suckless.org/patches/alpha_focus_highlight/) - Different transparency for focused window.
- [Box Draw](https://st.suckless.org/patches/boxdraw/) - Custom rendering of lines/blocks/braille characters for gapless alignment.
- [Scrollback](https://st.suckless.org/patches/scrollback/) - Add keyboard scroll back feature. All patches present on page are applied.
- [font2](https://st.suckless.org/patches/font2/) - Adds fallback fonts. **Be sure to use proper fallback font as `st` crashes when rendering gylph/special symobls. A good fallback font for this purpose could be [Symbola](https://fontlibrary.org/en/font/symbola).**
- [hidecursor](https://st.suckless.org/patches/hidecursor/) - Hides cursor when typing.
- [copyurl](https://st.suckless.org/patches/copyurl/) - Highlights and copies URL displayed on terminal.
- [clipboard](https://st.suckless.org/patches/clipboard/) - Copy and paste to system clipboard with keybinding and selection clipboard with mouse.
