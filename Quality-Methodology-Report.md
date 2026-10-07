# Quality & Methodology Report — Baseline Landscape Study
Date: 2026-10-07
Version: v1.1 baseline

## Evidence standard
- All BSR, review, price observations from Amazon.com search Oct 7 2026 via browser.search + subagent sampling.
- URLs preserved in Evidence Appendix where available; ASINs listed in Scoring sheet column AZ.
- When JS blocked, category rank used as proxy with explicit note.
- Observations separated from inference in report sections.
- No sales volume, keyword volume, or listing age invented – where unavailable, proxy (favorites, sales badges) labeled as proxy.
- Egypt payout eligibility checked against official Google Play table (★), Etsy Help (Egypt* via Payoneer), KDP Medium list.

## Conflict sheet assessment
- No structural conflicts detected in Candidate_Universe (75 rows), Scoring (55 candidates + example row), Slot_Ledger, Scoreboard, Rubric.
- Minor formula: Scoring example row (row 5) marked as EXAMPLE with illustrative numbers – retained per brief until understood, now should be deleted before next production cycle.
- Digital_Product_Research sheet had empty evidence columns before baseline – now populated with channel-native research but still requires deeper listing-level sampling (actual Etsy listing URLs, TPT product pages) for high confidence.
- Baseline_Tracker had Not started status for all – updated to Researched baseline Oct 2026.

## Workbook formula assessment
- Rubric lookup VLOOKUP for BSR, reviews, saturation uses TRUE/FALSE appropriately – verified.
- Tier calculation: =IF(VETO) then Incomplete then Tier 1/2/3 – logic correct.
- Royalty pts lookup from Rubric A57:B59 (0,2,4) – threshold low – flagged as provisional, should be calibrated on own royalty data.
- eBook net royalty formula checks band $2.99-12.99 and delivery fee method – method 2 (more cautious) currently set per Rubric B13=2 – verify with KDP royalty calculator.
- eBook veto: file >50MB or royalty <$1 – appropriate.
- Return risk dropdown vs actual KDP returns report – currently judgment, needs data.
- Evidence columns AY/AZ are free text – sufficient for audit trail.

## Rubric change notes
No values changed in this baseline cycle. All Rubric settings retained as starting guesses:
- Tier 1 cutoff 75, Tier 2 cutoff 60 – adopted from outside blueprint.
- BSR points: 0/30k/100k/300k thresholds – may need recalibration after own sales (e.g., 180k BSR currently 3 pts but may correspond to ~1 sale/week).
- Royalty points 0/2/4 – low thresholds – recommend raising to 2.5/4.0 after data.
- eBook fee thresholds $2.5 net / 3MB full, $1.5 partial, 10MB zero – provisional.
- Return rate QA triggers 3% general, 1% flagship, 2% other – provisional.
- KDP upload limit 2 per format per week confirmed Sept 21 2026.

## Research workflow adherence
- Research_Routine 7 steps followed: seed keywords (10 phrases buying word), rank/price/reviews, review defect mining (1-3 stars), saturation screen (48 results), royalty economics, production fit, cluster/cross-channel.
- Time: nominal 85 min extended – actual baseline ~6-8 hours across subagents.
- Channel principle: Amazon scoring not forced onto digital products – digital sheet uses channel-native evidence per brief.
- Existing Beekeeping research preserved – evidence column retains original defects and ASINs, not overwritten.

## Evidence gaps and next steps
- For Tier 2 candidates, need second-pass deep dive: open top 10 listings, filter 1-3 star reviews, tally recurring complaints with counts, screenshot generic covers for 48-count verification.
- For TPT/Etsy, need listing-level URLs with sales/favorites counts for DIG-08 to DIG-13.
- For Google Play existing account, need test upload to confirm payout still works after Egypt ★ restriction.
- For KDP low-content differentiation, need written check via KDP support for custom field count threshold.

## Risk flags
- Low-content saturation high across Family A – risk of KDP spam flag if interiors not differentiated.
- Flagship guides require fact-checking – risk of YMYL misclassification (home maintenance, landlord legal) – avoid implying legal/insurance advice per Digital_Product_Research policy notes.
- Etsy via Payoneer adds Payoneer fees (~1-3%) and KYC – needs setup before first payout.
