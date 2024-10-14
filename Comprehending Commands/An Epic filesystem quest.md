# An Epic filesystem quest

1)Used 'cd' to change directory wherever required
2)Used 'ls' or 'ls -a' to list out the files in given directories
3)Used 'cat' to read the contents of the file

```bash
hacker@commands~an-epic-filesystem-quest:~$ cd /
hacker@commands~an-epic-filesystem-quest:/$ ls
MEMO  boot       dev  flag  lib    lib64   media  nix  proc  run   srv  tmp  var
bin   challenge  etc  home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~an-epic-filesystem-quest:/$ cat MEMO
Great sleuthing!
The next clue is in: /opt/ghidra/Ghidra/Features/Base/data/typeinfo/generic
hacker@commands~an-epic-filesystem-quest:/$ cd /opt/ghidra/Ghidra/Features/Base/data/typeinfo/generic
hacker@commands~an-epic-filesystem-quest:/opt/ghidra/Ghidra/Features/Base/data/typeinfo/generic$ ls
NUGGET  generic_clib.gdt  generic_clib_64.gdt
hacker@commands~an-epic-filesystem-quest:/opt/ghidra/Ghidra/Features/Base/data/typeinfo/generic$ cat NUGGET
Tubular find!
The next clue is in: /usr/share/icons/hicolor/36x36/actions

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/opt/ghidra/Ghidra/Features/Base/data/typeinfo/generic$ cd /usr/share/icons/hicolor/36x36/actions
hacker@commands~an-epic-filesystem-quest:/usr/share/icons/hicolor/36x36/actions$ ls -a
.  ..  .ALERT
hacker@commands~an-epic-filesystem-quest:/usr/share/icons/hicolor/36x36/actions$ cat .ALERT
Great sleuthing!
The next clue is in: /usr/share/icons/hicolor/24x24/stock/data

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/usr/share/icons/hicolor/36x36/actions$ cd /usr/share/icons/hicolor/24x24/stock/data
hacker@commands~an-epic-filesystem-quest:/usr/share/icons/hicolor/24x24/stock/data$ ls
NOTE
hacker@commands~an-epic-filesystem-quest:/usr/share/icons/hicolor/24x24/stock/data$ cat NOTE
Yahaha, you found me!
The next clue is in: /usr/local/lib/python3.8/dist-packages/ipywidgets/widgets/tests

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/usr/share/icons/hicolor/24x24/stock/data$ ls -a /usr/local/lib/python3.8/dist-packages/ipywidgets/widgets/tests
.                             test_interaction.py         test_widget_box.py             test_widget_string.py
..                            test_link.py                test_widget_button.py          test_widget_templates.py
.LEAD                         test_selectioncontainer.py  test_widget_datetime.py        test_widget_time.py
__init__.py                   test_send_state.py          test_widget_float.py           test_widget_upload.py
__pycache__                   test_set_state.py           test_widget_image.py           utils.py
data                          test_traits.py              test_widget_naive_datetime.py
test_datetime_serializers.py  test_utils.py               test_widget_output.py
test_docutils.py              test_widget.py              test_widget_selection.py
hacker@commands~an-epic-filesystem-quest:/usr/share/icons/hicolor/24x24/stock/data$ cat /usr/local/lib/python3.8/dist-packages/ipywidgets/widgets/tests/.LEAD
Congratulations, you found the clue!
The next clue is in: /usr/lib/python3/dist-packages/jedi/third_party/typeshed/third_party/2/six/moves/urllib

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/usr/share/icons/hicolor/24x24/stock/data$ cd /usr/lib/python3/dist-packages/jedi/third_party/typeshed/third_party/2/six/moves/urllib
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/jedi/third_party/typeshed/third_party/2/six/moves/urllib$ ls
DISPATCH  __init__.pyi  error.pyi  parse.pyi  request.pyi  response.pyi  robotparser.pyi
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/jedi/third_party/typeshed/third_party/2/six/moves/urllib$ cat DISPATCH
Yahaha, you found me!
The next clue is in: /usr/lib/python3/dist-packages/sage/typeset

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/jedi/third_party/typeshed/third_party/2/six/moves/urllib$ ls /usr/lib/python3/dist-packages/sage/typeset
SECRET-TRAPPED  __pycache__  ascii_art.py      character_art_factory.py  unicode_art.py
__init__.py     all.py       character_art.py  symbols.py
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/jedi/third_party/typeshed/third_party/2/six/moves/urllib$ cat /usr/lib/python3/dist-packages/sage/typeset/SECRET-TRAPPED
Congratulations, you found the clue!
The next clue is in: /usr/lib/python3/dist-packages/sympy/physics/mechanics

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/jedi/third_party/typeshed/third_party/2/six/moves/urllib$ ls /usr/lib/python3/dist-packages/sympy/physics/mechanics
DOSSIER-TRAPPED  __pycache__  functions.py  lagrange.py   models.py    rigidbody.py  tests
__init__.py      body.py      kane.py       linearize.py  particle.py  system.py
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/jedi/third_party/typeshed/third_party/2/six/moves/urllib$ cat /usr/lib/python3/dist-packages/sympy/physics/mechanics/DOSSIER-TRAPPED
Great sleuthing!
The next clue is in: /usr/lib/python3/dist-packages/sympy/printing/tests

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/jedi/third_party/typeshed/third_party/2/six/moves/urllib$ ls -a /usr/lib/python3/dist-packages/sympy/printing/tests
.              test_codeprinter.py  test_gtk.py         test_maple.py        test_preview.py  test_str.py
..             test_conventions.py  test_jscode.py      test_mathematica.py  test_pycode.py   test_tableform.py
.REVELATION    test_cxxcode.py      test_julia.py       test_mathml.py       test_python.py   test_tensorflow.py
__init__.py    test_dot.py          test_lambdarepr.py  test_numpy.py        test_rcode.py    test_theanocode.py
__pycache__    test_fcode.py        test_latex.py       test_octave.py       test_repr.py     test_tree.py
test_ccode.py  test_glsl.py         test_llvmjit.py     test_precedence.py   test_rust.py
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/jedi/third_party/typeshed/third_party/2/six/moves/urllib$ cat /usr/lib/python3/dist-packages/sympy/printing/tests/.REVELATION
CONGRATULATIONS! Your perserverence has paid off, and you have found the flag!
It is: pwn.college{sLJ5zAHg_hsCcRaA1rrq_wme35K.dljM4QDL0czM2czW}
```

The resources used were
1)Ubuntu 22.04.5 LTS
2)pwn.college
