# r/CryptoCurrency Moon Distribution Dataset

Every 4 weeks, the subreddit r/CryptoCurrency distributions a cryptocurrency called Moons to its contributing users based on the karma they received during that 4 week period (with additional modifiers). Within the `/data/` directory contains the karma each user had during each 4 week interval that is used to determine how many Moons they'll receive. Each user within each CSV file will have a karma that then gets converted to Moons based on some ratio. The ratios, if available, are contained in `metadata.yaml` along with a source if available. Some rounds do not have Moon-to-Karma ratios.

## Notes

- Within `metadata.yaml` are links to the CSV files that are hosted by Reddit. Some of the URLs, particularly the older ones, will return an error stating that your access has been denied (e.g., [round 24](https://reddit-meta-production.s3.amazonaws.com/distribution/publish/CryptoCurrency/round_24_finalized.csv)). Some of these rounds are recoverable through the [Wayback Machine](https://web.archive.org/), but some are not (e.g., round 1 and 3). Files that were not recovered from the Wayback Machine were sourced from the moderators of r/CryptoCurrency.

- Each ratio within the `metadata.yaml` file were sourced by hand from comments made within the thread. Some threads (e.g., round 3) do not have a comment specifying what the Moon-to-Karma ratio was and need to be derived in some other way.

## Acknowledgments

I appreciate the moderators of r/CryptoCurrency, particularly u/IHaventEvenGotADog, for responding to my DM giving me the missing data that couldn't be recovered through the Wayback Machine.