# PDFSearcher
Allows the parsing, fuzzy searching, and opening of PDF files. Works on Mac OSX. I built this to effectively search through class slides for an open book college exam. 

# Usage
Run `pdfsearch` in a directory to start. You can look at the fzf documentation for more information on specific search commands. If you find a line in a pdf you would like to open, press enter and it will open the pdf to the specified page.

# Dependencies
- [ripgrep-all](https://github.com/phiresky/ripgrep-all)
- [fzf](https://github.com/junegunn/fzf)
- [pandoc](https://github.com/jgm/pandoc)

### Brew Dependency Installation
If on mac, both can be installed with Homebrew
```bash
brew install rga fzf pandoc
```

# Setup
```bash
git clone git@github.com:tmcnitt/PFSearcher.git

# Make pdf preview runnable
sudo chmod +x "./PDFSearcher/pdfpreview"

# If using bash
echo "source $(pwd)/PDFSearcher/pdfsearch" >> ~/.bash_profile
echo "export PATH=\$PATH:$(pwd)/PDFSearcher" >> ~/.bash_profile

# If using zsh
echo "source $(pwd)/PDFSearcher/pdfsearch" >> ~/.zshrc
echo "export PATH=\$PATH:$(pwd)/PDFSearcher" >> ~/.zshrc
```

# License
Copyright 2022 Troy McNitt

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
