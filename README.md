# Bylaws of Sigma Zeta

[![Build status](https://ci.appveyor.com/api/projects/status/ds252p7v6mdc2d8m?svg=true)](https://ci.appveyor.com/project/lcamichigan/chapter-bylaws)
[![Build Status](https://travis-ci.org/lcamichigan/chapter-bylaws.svg?branch=tex)](https://travis-ci.org/lcamichigan/chapter-bylaws)

This is a collection of resources for maintaining the collegiate bylaws of
[Sigma Zeta of ΛΧΑ](https://lcamichigan.com).

## Getting Started

To make leases, you need [LuaTeX](http://www.luatex.org), which is free and
cross-platform. You also need the font
[Lib­ert­i­nus](https://github.com/libertinus-fonts/libertinus). This is also free,
and you’ll get it automatically when you install LuaTeX.

### On Windows

The most reliable way to install LuaTeX is probably to install
[TeX Live](https://www.tug.org/texlive/). To install TeX Live, visit
https://www.tug.org/texlive/acquire-netinstall.html, and then download and run
install-tl-windows.exe. Note that installing TeX Live can take a few hours.

### On macOS

The easiest way to install LuaTeX is probably to install
[MacTeX](https://www.tug.org/mactex/). To install MacTeX, visit
https://tug.org/mactex/mactex-download.html, download MacTeX.pkg, and then
double-click MacTeX.pkg.

## Making a Bylaws PDF File

To create a PDF file of the Bylaws, enter in PowerShell:

```powershell
foreach ($i in 1..2) { lualatex Bylaws.tex }
```

or in Command Prompt:

```batch
for /l %G in (1, 1, 2) do lualatex Bylaws.tex
```

or in Terminal:

```sh
for i in {1..2}; do lualatex Bylaws.tex; done
```
