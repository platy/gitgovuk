# UK Government advice and publications

__No longer updated__: eventually, after several years it was clear how unsuitable git was for this data, the data is still being collected by the website at https://govdiff.njk.onl, but it using a different backend storage.

This is a mirror in git of publications and guidance from the UK government provided at www.gov.uk. The files are generally those related to Brexit and the purpose is to enable usr to see haw the advise has changed using diffs.

I made this because I was tired of seeing that guidance relevant to me was updated on www.gov.uk and not being able to find what had changed in very long documents.

## Disclaimer

I am not associated with the UK Government and information here is not necessarily up to date, please see www.gov.uk

This is currently only being updated when Brexit info changes, documents changed for other reasons will not be updated.

## License

All content is produced by the UK Government unless otherwise stated and is released under the [Open Government License](https://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/).

## Method

The repository is pre-populated with a bunch of pages awkwardly scraped from www.gov.uk starting with the brexit page using wget `wget --recursive -l 2 --no-parent https://www.gov.uk/government/brexit`

Each of the docs is stripped of its headers and footers and down to just the `<main id="content">` element.

Emails received from the [Brexit email subscription](https://www.gov.uk/email-signup/?topic=/government/brexit) cause pages to be updated and provide the commit messages for the updates.
