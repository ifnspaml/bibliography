# Bibliography
Group bibliography

## Workflows and Best Practices
Please pull a fresh version of this repository when you start to write a new paper and use `ifn_spaml_bibliography.bib` as your bibliography. After submission and review of the paper please commit your new corrected references here. 

#### Merge Conflicts

In the case that someone added references in between and you run into a merge conflict, please use a merge editor of your choice, to compare your local `ifn_spaml_bibliography.bib` with the most recent `ifn_spaml_bibliography.bib` from this repository. 

#### Check for duplicates
You can use the following tool, to check if duplicates are in the .bib file. 

https://flamingtempura.github.io/bibtex-tidy/

Paste the raw text of the `ifn_spaml_bibliography.bib` file inside the web-tool and check if there are duplicates names. Then please search and edit them **manually** inside your text editor. Please do only search for duplicate bibtex keys (e.g., Klingner2020). If duplicate entries are found please append the next unused `[a-z]` letter to one of the keys. Do not commit the version from *tidy* web-tool, as it is not confirmed that it won't corrupt some entries. 

#### Provide Surnames

Some conferences require the full surnames of the authors. So if you add references please provide surnames of all authors.


## Templates
Do not add abstracts or reviews.

Conference papers:
```LaTeX
@InProceedings{AuthorPublicationYear[a-z],
  author      = {Max Musterfrau and Jane Doe and Olaf Normalverbraucherin},
  title       = {{Title Using Headline Capitalization}},
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
  author    = {Max Musterfrau and Jane Doe and Olaf Normalverbraucherin},
  title     = {{Title Using Headline Capitalization}},
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
  author        = {Max Musterfrau and Jane Doe and Olaf Normalverbraucherin},
  title         = {{Title Using Headline Capitalization}},
  journal       = {arXiv},
  year          = {XXXX},
  month         = [jan,feb,mar,apr,may,jun,jul,aug,sep,oct,nov,dec],
  archiveprefix = {arXiv},
  eprint        = {XXXX.XXXXX}, # e-print number
  keywords      = {Keyword1; Keyword2; ...},
}
```
*Headline Capitalization: Capitalize words with four or more letters.*

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
