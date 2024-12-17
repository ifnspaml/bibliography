# Bibliography
Group bibliography, please read this README carefully.

## Workflows and Best Practices
Please pull a fresh version of this repository when you start to write a new paper and use `ifn_spaml_bibliography.bib` as your bibliography. After submission and review of the paper please commit your new corrected references here. 

#### Merge Conflicts
In the case that someone added references in between and you run into a merge conflict, please use a merge editor of your choice, to compare your local `ifn_spaml_bibliography.bib` with the most recent `ifn_spaml_bibliography.bib` from this repository. 

#### Formatting
If bibtex keys are already in use please append the next unused `[a-z]` letter to your key.

Before commiting please use the following tool to tidy up your .bib file. 

[https://flamingtempura.github.io/bibtex-tidy/](https://flamingtempura.github.io/bibtex-tidy/index.html?opt=%7B%22modify%22%3Atrue%2C%22curly%22%3Afalse%2C%22numeric%22%3Afalse%2C%22months%22%3Afalse%2C%22space%22%3A2%2C%22tab%22%3Afalse%2C%22align%22%3A16%2C%22sort%22%3A%5B%22key%22%5D%2C%22stripEnclosingBraces%22%3Afalse%2C%22dropAllCaps%22%3Afalse%2C%22escape%22%3Afalse%2C%22sortFields%22%3A%5B%22title%22%2C%22author%22%2C%22journal%22%2C%22booktitle%22%2C%22shorttitle%22%2C%22year%22%2C%22volume%22%2C%22number%22%2C%22pages%22%2C%22address%22%2C%22month%22%2C%22day%22%2C%22location%22%2C%22on%22%2C%22publisher%22%2C%22series%22%2C%22doi%22%2C%22isbn%22%2C%22issn%22%2C%22url%22%2C%22urldate%22%2C%22copyright%22%2C%22category%22%2C%22metadata%22%2C%22keywords%22%5D%2C%22stripComments%22%3Afalse%2C%22trailingCommas%22%3Afalse%2C%22encodeUrls%22%3Afalse%2C%22tidyComments%22%3Atrue%2C%22removeEmptyFields%22%3Afalse%2C%22removeDuplicateFields%22%3Afalse%2C%22lowercase%22%3Afalse%2C%22backup%22%3Atrue%7D)

The current bibliography has been formatted with the following parameter set:
```
bibtex-tidy --align=16 --sort=key --no-escape --sort-fields=title,author,journal,booktitle,shorttitle,year,volume,number,pages,address,month,day,location,on,publisher,series,doi,isbn,issn,url,urldate,copyright,category,metadata,keywords --no-remove-dupe-fields --no-lowercase YOUR_FILE.bib
```

Paste the raw text of the `ifn_spaml_bibliography.bib` file inside the linked web-tool tidy it up. Before commiting then please review your new entries and changes **manually** with a diff tool of your choice. 

#### Headline Capitalization
Capitalize all words with four or more letters.*

#### Provide Surnames

Some conferences require the full surnames of the authors. So if you add references please provide surnames of all authors. Avoid using "and others" in your author list to generate "et al.". There are bibtex/biber options to do that.

## Templates
Do not add abstracts or reviews.

Conference papers:
```LaTeX
@InProceedings{AuthorPublicationYear[a-z],
  title       = {{Title Using Headline Capitalization}},
  author      = {Max Musterfrau and Jane Doe and Olaf Normalverbraucherin},
  booktitle   = {Proc. of CONF},
  year        = {xxxx},
  pages       = {xxxx--xxxx},
  address     = {City, (State,) Country},
  month       = [jan,feb,mar,apr,may,jun,jul,aug,sep,oct,nov,dec],
  keywords    = {Keyword1; Keyword2; ...},
}
```

Journal arcticles:
```LaTeX
@Article{AuthorPublicationYear[a-z],
  title     = {{Title Using Headline Capitalization}},
  author    = {Max Musterfrau and Jane Doe and Olaf Normalverbraucherin},
  journal 	= {IEEE Transactions on Lorem Ipsum (ABBR.)},
  year      = {xxxx},
  volume    = {xx},
  number    = {x},
  pages     = {xxxx--xxxx},
  month     = [jan,feb,mar,apr,may,jun,jul,aug,sep,oct,nov,dec],
  keywords  = {Keyword1; Keyword2; ...},
}
```

ITU standard:
```LaTeX
@Manual{ITU[0-9]{0,4},
  title                    = {{Rec. P.1110: Wideband Hands-Free Communication in Motor Vehicles}},
  author                   = {{ITU}},
  month                    = [jan,feb,mar,apr,may,jun,jul,aug,sep,oct,nov,dec],
  organization             = {{International Telecommunication Union, Telecommunication Standardization Sector (ITU-T)}},
  year                     = {xxxx},
}
```

Homepage:
```LaTeX
@Misc{SciPy,
  title                    = {{SciPy: Open Source Scientific Tools for Python}},
  author                   = {Eddy Jones and Thomas Oliphant and Peter Peterson and others},
  note                     = {[Online; accessed <today>]},
  year                     = {2001--},
  url                      = {http://www.scipy.org/}
}
```

Book:
```LaTeX
@Book{AuthorPublicationYear[a-z],
  title     = {Deep Lorem Ipsum with PyTorch},
  publisher = {Publisher Name},
  year      = {XXXX},
  author    = {Max Musterfrau and Jane Doe and Olaf Normalverbraucherin},
  keywords  = {Keyword1; Keyword2; ...},
}
```
arXiv e-Print:
```LaTeX
@Article{AuthorPublicationYear[a-z],
  title         = {{Title Using Headline Capitalization}},
  author        = {Max Musterfrau and Jane Doe and Olaf Normalverbraucherin},
  journal       = {arXiv},
  year          = {XXXX},
  month         = [jan,feb,mar,apr,may,jun,jul,aug,sep,oct,nov,dec],
  archiveprefix = {arXiv},
  eprint        = {XXXX.XXXXX}, # e-print number
  keywords      = {Keyword1; Keyword2; ...},
}
```


## Abbreviations for commonly used conferences
| Conference                                                   | booktitle in bibtex  |
| ------------------------------------------------------------ | -------------------- |
| National Conference on Artificial Intelligence               | Proc. of AAAI        |
| IEEE Automatic Speech Recognition and Understanding Workshop | Proc. of ASRU        |
| British Machine Vision Conference                            | Proc. of BMVC        |
| Conference on Computer Vision and Pattern Recognition        | Proc. of CVPR        |
| European Conference on Computer Vision                       | Proc. of ECCV        |
| IEEE International Conference on Acoustics, Speech and Signal Processing | Proc. of ICASSP      |
| International Conference on Computer Vision                  | Proc. of ICCV        |
| IEEE International Confernence on Image Processing           | Proc. of ICIP        |
| International Conference on Learning Representations         | Proc. of ICLR        |
| International Conference on Machine Learning                 | Proc. of ICML        |
| Annual Conference of the International Speech Communication Association | Proc. of Interspeech |
| IEEE Intelligent Transportation Systems Conference           | Proc. of ITSC        |
| IEEE Intelligent Vehicles Symposium                          | Proc. of IV          |
| Conference on Neural Information Processing Systems          | Proc. of NeurIPS     |
| IEEE Workshop on Applications of Signal Processing to Audio and Acoustics | Proc. of WASPAA      |
| International Workshop on Acoustic Signal Enhancement        | Proc. of IWAENC      |
| European Signal Processing Conference                        | Proc. of EUSIPCO     |
| IEEE Winter Conference on Applications of Computer Vision    | Proc. of WACV        |

*For workshops that were in conjunction with a conference add " - Workshops" to the booktitle, e.g., "Proc. of CVPR - Workshops"*
