# New York City Directories

[![Join the chat at https://gitter.im/nypl-spacetime/city-directories](https://badges.gitter.im/nypl-spacetime/city-directories.svg)](https://gitter.im/nypl-spacetime/city-directories?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

The New York Public Library has [digitized its collection of city directories](https://www.nypl.org/blog/2016/09/21/new-york-city-directories-free-online), and the resulting high-resolution images can be browsed and downloaded on our [Digital Collections](https://digitalcollections.nypl.org/collections/new-york-city-directories#/?tab=about).

As part of the the [NYC Space/Time Directory](http://spacetime.nypl.org/) project and in collaboration with the New York University, we are using optical character recognition (OCR) to turn the city directories into a searchable atlas of historical New York City.

## Meetups

Two meetups have been organized about the digitized city directories:

- [City Directories: 137 years of NYC History](https://www.meetup.com/historical-data-and-maps-at-nypl/events/235450812/)
- [Extracting a Million-Record Dataset from Historical NYC City Directories](https://www.meetup.com/historical-data-and-maps-at-nypl/events/244290064/) ([slides](http://spacetime.nypl.org/city-directory-meetup))

## List of digitized city directories

See [`DIRECTORIES.md`](DIRECTORIES.md) for a table of the city directories we are processing and extracting text from. To just browse and download the scanned books, visit [Digitial Collections](https://digitalcollections.nypl.org/collections/new-york-city-directories#/?tab=about).

## Data

__Processed city directory data will soon be published on the NYC Space/Time Directory homepage!__

## hOCR files

__hOCR files will soon be published in our data repository!__

Anatomy of an hOCR file name:

Example:

    1849.00030.28.56749967.e10e9aa0-5291-0134-79ba-00505686a51c.processed.hocr

- `1849` ⟶ year of directory
- `00030` ⟶ page number of original print page
- `28` ⟶ image number of sequentially downloaded images from single item (i.e. a directory)
- `56749967` ⟶ NYPL asset's individual image ID
- `e10e9aa0-5291-0134-79ba-00505686a51c` ⟶ NYPL UUID for individual image
- `processed` ⟶ image was preprocessed by ImageMagick textcleaner

## Open source libraries

- https://github.com/tesseract-ocr/tesseract
- https://github.com/nypl-spacetime/city-directory-entry-parser
- https://github.com/nypl-spacetime/hocr-detect-columns
