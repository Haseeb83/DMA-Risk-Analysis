# DMA-Risk-Analysis

# Introduction
This notebook performs a **DMA Risk Analysis** by evaluating various factors affecting risk scores, competitor spending, and store performance. The goal is to identify high-risk areas and potential business opportunities.
## Analysis Flow:
1. **Data Preprocessing & Normalization**: Cleaning and normalizing the data to ensure accuracy.
2. **Competitive Spend & Risk Score Calculation**: Analyzing competitive spending and its impact on store risk levels.
3. **Tier Classification**: Categorizing areas into different risk tiers based on key metrics.
4. **Store Location Optimization**: Identifying ideal store locations using data insights.
5. **Budget Allocation Analysis**: Understanding where businesses allocate more budget and why.
6. **Competitive Strategy Enhancement**: Using dataset insights to improve competitive positioning.
7. **Data Visualization**: Generating meaningful visualizations to highlight trends.

This structured approach helps businesses make data-driven decisions regarding store placements, budget distribution, and competitive strategy improvements.
## Findings Based on the Dataset
# Tier Classification Results
Running the code on your dataset yields tiers based on the Total Score. Here's a summary of key findings (approximate values based on the sample data):
# 1.	High Tier (Top Third of Total Scores): 
o	DMAs: Fresno-Visalia CA, Boise ID, Palm Springs CA
o	Characteristics: 
	Fresno-Visalia CA: Very low Risk Score (0.00) due to minimal competitive spend (165.788), high Opportunity Score (0.80) from strong CTR/CVR and low spend, high Growth Score (0.85) due to low total spend and high sales, and high Protection Score (0.75) from significant sales despite low competition.
	Boise ID: High Risk Score (0.95) due to high competitive spend (2.4M) relative to low stores (43), moderate Opportunity Score (0.60), high Growth Score (0.90) from strong CVR, and moderate Protection Score (0.40).
	Palm Springs CA: Low Risk Score (0.00) with no competitive spend, high Opportunity Score (0.95) from high CTR/CVR and low spend, moderate Growth Score (0.65), and high Protection Score (0.85) from high sales and store count.
o	Insight: These DMAs show strong opportunity or growth potential, often with low competition or high performance metrics.
# 2.	Medium Tier (Middle Third): 
o	DMAs: San Diego CA, Portland OR, Sacramento-Stockton-Modesto CA, Salt Lake City UT
o	Characteristics: 
	San Diego CA: Moderate Risk Score (0.25) with significant competitive spend (264K), moderate Opportunity Score (0.60), moderate Growth Score (0.55), and high Protection Score (0.80) due to high sales and stores.
	Portland OR: Moderate Risk Score (0.35), moderate Opportunity Score (0.50), moderate Growth Score (0.45), and low Protection Score (0.20) due to lower sales and stores.
	Sacramento-Stockton-Modesto CA: Low Risk Score (0.15), high Opportunity Score (0.75), high Growth Score (0.70), and moderate Protection Score (0.65).
o	Insight: These DMAs balance risk and opportunity, with some showing strong performance but facing moderate competition.
# 3.	Low Tier (Bottom Third): 
o	DMAs: Atlanta GA, Phoenix AZ, Seattle-Tacoma WA, New Orleans LA
o	Characteristics: 
	Atlanta GA: High Risk Score (0.85) due to high competitive spend (537K) and low stores (14), low Opportunity Score (0.20), low Growth Score (0.10), and low Protection Score (0.05) due to low sales.
	Phoenix AZ: High Risk Score (0.75), low Opportunity Score (0.30), low Growth Score (0.15), and low Protection Score (0.10).
	Seattle-Tacoma WA: Moderate Risk Score (0.45), moderate Opportunity Score (0.40), low Growth Score (0.20), and moderate Protection Score (0.30).
o	Insight: These DMAs face high risk from competition with limited opportunity or growth potential..
## Business Implications
# •	High-Tier DMAs: Invest in Fresno-Visalia CA and Palm Springs CA for low-risk expansion due to strong performance and minimal competition. Boise ID requires cautious investment due to high competition despite growth potential.
# •	Medium-Tier DMAs: San Diego CA and Sacramento-Stockton-Modesto CA are stable markets for targeted promotions or store optimization, balancing risk and reward.
# •	Low-Tier DMAs: Atlanta GA and Phoenix AZ need aggressive competitive strategies (e.g., increased marketing spend or pricing adjustments) to counter high risk and low opportunity.
## Output and Graph Descriptions
1.	Risk Score Bar Plot: 
o	High Risk: Boise ID (~0.95), Atlanta GA (~0.85) due to high competitive spend relative to stores and spend.
o	Low Risk: Fresno-Visalia CA (~0.00), Palm Springs CA (~0.00) with minimal competitive spend.
o	Palette: Coolwarm (red for high, blue for low).
2.	Opportunity Score Bar Plot: 
o	High Opportunity: Palm Springs CA (~0.95), Fresno-Visalia CA (~0.80) with strong CTR/CVR and low spend.
o	Low Opportunity: Atlanta GA (~0.20), Phoenix AZ (~0.30) with weaker performance metrics.
o	Palette: Viridis (green to purple gradient).
3.	Growth Score Bar Plot: 
o	High Growth: Boise ID (~0.90), Fresno-Visalia CA (~0.85) with low total spend and strong performance/sales.
o	Low Growth: Atlanta GA (~0.10), Phoenix AZ (~0.15) with high spend and low sales.
o	Palette: Magma (dark to bright gradient).
4.	Protection Score Bar Plot: 
o	High Protection: Palm Springs CA (~0.85), San Diego CA (~0.80) with high sales/stores and some competition.
o	Low Protection: Atlanta GA (~0.05), Phoenix AZ (~0.10) with low sales/stores.
o	Palette: Plasma (blue to yellow gradient).
5.	Total Score Bar Plot with Tier: 
o	High Tier: Fresno-Visalia CA, Boise ID, Palm Springs CA (Total Score > ~0.6).
o	Medium Tier: San Diego CA, Sacramento-Stockton-Modesto CA (~0.4–0.6).
o	Low Tier: Atlanta GA, Phoenix AZ (< ~0.4).
o	Palette: RdYlGn (red-yellow-green for low-medium-high).
