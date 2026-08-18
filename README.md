HOW TO USE THIS TRACKER


The 'Articles' tab is where you log every new item. Fill one row per article.
Region and Sentiment columns have dropdowns already (Data > Data validation).
Tag columns (SDGs, Africa, etc.) are 1/0 flags. In Sheets, select the tag
   columns and go to Format > Data validation > Criteria: Checkbox, to turn them into
   real checkboxes (TRUE/FALSE) if you prefer clicking over typing 1.
The summary tabs (Region Summary, Tag Summary, Sentiment Summary, Sentiment Over Time)
   use COUNTIF/AVERAGEIFS formulas that point at the Articles tab. They update
   automatically as you add rows - just make sure new rows stay inside the formula range
   (ranges are set to row 1000 to leave headroom; extend if you exceed that).
To keep a Datawrapper chart live: File > Share > Publish to web > select a summary tab
   > CSV. Paste that published CSV URL into Datawrapper's 'External data' or use
   'Refresh data' > paste URL. The chart will re-pull whenever you edit the sheet.
Add new tags by inserting a new column in 'Articles' (after the last tag column) and
   adding a matching row in 'Tag Summary'. Add new regions/sentiments by editing the
   'Lists' tab - dropdowns reference it automatically.

TAB GUIDE
- Articles: log one row per article. This is the only tab you manually edit regularly.
- Region Summary: count of articles per region, dropdown source values for Region and Sentiment. auto-updating.
- Tag Summary: count of articles per tag, auto-updating.
- Sentiment Summary: count of articles per sentiment category, auto-updating.
- Sentiment Over Time: monthly average sentiment score, auto-updating - feed this to a
  Datawrapper line chart to track tone over time.

NOTE: Sentiment mapping is done by comparing the article to those in the existing dataset. It does not use
a sentiment mapping model.

Score the SDG / post-2030 progress being described, not the geopolitics around it.
A piece can criticize a country and still be Neutral if it takes no position on
whether the goals themselves are succeeding.

Positive - frames progress, opportunity, or momentum (transformation, leadership,
breakthrough, collaboration, opportunity). Usually reads as a pitch: a plan,
declaration, or commitment is the news.

Neutral - reports facts, process, or diplomacy without a clear lean (remarks,
meeting summaries, procedural updates, frameworks/models being described).

Negative - flags failure, stalling, urgency, or criticism (stalled, regressing,
running out of time, retreat, failure, gap). Usually reads as a warning.

Quick test: if the headline alone tells you the tone, tag it fast. If you have to
read the summary twice, it is probably Neutral - do not force a lean that is not there.

Regression + transformation in the same piece: tag the forward-looking claim, not
the backward-looking diagnosis. Bad stats + a real plan to fix them = Positive.
Bad stats + no real plan (or a plan going nowhere) = Negative. Only use Neutral
when the regression and the transformation are genuinely balanced, not as a default.

The plan is to host this on github for a shareable tracker.
For any questions, please reach out to Aiza or others from the SDI team.




