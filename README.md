# centenary-research-engine

A Python research toolkit for gathering and analysing digital evidence of UK First World War centenary commemoration (2014 to 2018). Built to support a PhD thesis examining the power, networks, and politics of commemoration at Queen Mary University of London.

## What this does

The notebook collects structured digital evidence across two primary data streams:

**YouTube Data API v3** — retrieves commemorative video content, enriches results with view counts, like counts, and comment counts, and outputs a ranked CSV by engagement. Captures public reach and audience response to official and unofficial centenary content.

**Guardian Open Platform API** — fetches news articles from the Guardian by commemorative period and date range. Captures volume of coverage, section distribution (news, opinion, culture), byline data, and word count. Outputs to CSV and a full title list with URLs.

**Google Custom Search API** — searches for centenary coverage across 12 named UK news and heritage sources by commemorative period and site. Sources include the Guardian, Telegraph, BBC, Daily Mail, Times, Independent, Mirror, ITV, History Extra, Imperial War Museum, Yorkshire Post, and Harrogate Advertiser. Designed to surface elite national and local press coverage side by side.

## Research context

The thesis is titled *The Power, People and Politics of Commemoration through the Centenary of the First World War*. The digital evidence strand interrogates the online visibility of key commemorative moments across five periods:

- Outbreak centenary, August 2014
- Tower of London Poppies (Blood Swept Lands and Seas of Red), October to November 2014
- Somme centenary, July 2016
- Passchendaele centenary, 2017
- Armistice centenary, November 2018

The central analytical tension is between elite-curated commemoration (state, institutions, national press) and grassroots participation (local press, public engagement, YouTube). The engine is designed to generate quantitative evidence that complements qualitative archival and interview-based research.

## Key methodological note

This approach engages directly with what the thesis terms the "denominator problem" in digital history: the difficulty of interpreting engagement metrics without knowing the total population of relevant content. The engine is designed to generate comparable, bounded datasets across periods and sources rather than claim representativeness.

## Stack

- Python 3 (Google Colab)
- YouTube Data API v3
- Guardian Open Platform API
- Google Custom Search JSON API
- SerpApi (news search layer)
- requests, csv, json, collections

## Output files

- `youtube_centenary.csv` — video results ranked by view count with engagement stats
- `news_centenary.csv` — news results by period and source
- `guardian_centenary.csv` — Guardian articles by period with byline, section, word count
- `guardian_titles.txt` — full title list with publication dates and URLs

## Status

Active development. Currently integrating Guardian API and Google Custom Search outputs for comparative period analysis.

## Academic context

Part-time PhD, Queen Mary University of London, supervised 2020 to 2025 (expected completion). Chicago referencing throughout. Thesis uses this digital evidence strand alongside archival research, elite network analysis, and interview data including testimony from senior figures in the UK commemoration programme.
