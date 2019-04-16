# bibliography
Group bibliography

Define some syntax here, e.g.,: Key: AuthorPublicationYear[a-z], Pages: {123--125}

Do not add abstracts or reviews.

Conference papers:
```LaTeX
@InProceedings{AuthorPublicationYear[a-z],
  author      = {M. Musterfrau and J. Doe and O. Normalverbraucherin},
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
  author    = {M. Musterfrau and J. Doe and O. Normalverbraucherin},
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
  author                   = {E. Jones and T. Oliphant and P. Peterson and others},
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
  author    = {M. Musterfrau and J. Doe and O. Normalverbraucherin},
  keywords  = {Keyword1; Keyword2; ...},
}
```
arXiv e-Print:
```LaTeX
@Article{AuthorPublicationYear[a-z],
  author        = {M. Musterfrau and J. Doe and O. Normalverbraucherin},
  title         = {{Title Using Headline Capitalization}},
  journal       = {arXiv},
  year          = {XXXX},
  month         = [jan,feb,mar,apr,may,jun,jul,aug,sep,oct,nov,dec],
  archiveprefix = {arXiv},
  eprint        = {XXXX.XXXXX}, # e-print number
  keywords      = {Keyword1; Keyword2; ...},
}
```
