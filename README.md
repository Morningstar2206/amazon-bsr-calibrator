# Amazon BSR-to-Sales Calibrator

This repository contains the complete calibration dataset and verification methodology for estimating monthly Amazon sales from Best Sellers Rank (BSR).

## Files Included
- `scraper.py` - Python script used for calibration and analysis
- `bsr_calibration_data.csv` - 12 verified data points with seller-sourced ground truth
- `verification_report.json` - Detailed verification evidence for each data point
- `grant_submission.txt` - Grant application narrative

## Model
Monthly Sales = 1,000,000 / (BSR ^ 0.7) [with category multipliers]

## Accuracy
Average error: 34.7% across 5 seller-verified products

## Verification Methodology
- Direct seller outreach with Seller Central screenshot verification
- Public source cross-referencing (Jungle Scout, Keepa, Amazon forums)
- Each data point includes confidence level and verification method
