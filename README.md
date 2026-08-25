# E-commerce Business Analysis

Analysis of a public e-commerce dataset, from raw tables to business
recommendations. Six questions a marketing and operations team would actually
ask, answered with SQL, Python and Tableau.

**[Read the full presentation (PDF)](slides/ecommerce_business_analysis.pdf)**

## The dataset

`bigquery-public-data.thelook_ecommerce` on Google BigQuery: a public dataset
covering users, orders, order items, products and traffic sources for a
fictional apparel retailer.

Data was queried in BigQuery, exported to CSV, cleaned in Python with Pandas and
NumPy (removing null and duplicate records, casting types, sorting and reindexing),
then visualized in Tableau, one dashboard per question.

## What I looked at, and what I found

### Where loyal customers come from

Email is the leading traffic source for returning customers, with AdWords close
behind: retention here runs on direct, personalized messaging rather than on
reach. Organic traffic is disproportionately low, which makes SEO the clearest
underexploited investment. YouTube and Facebook sit in the middle, with reach
that is not converting into loyalty.

### Where buyers are

Strong concentration in China and the United States, with a meaningful presence
across Latin America. European markets and Asian countries other than China are
underrepresented relative to their size, and are the natural place to expand.

### Who they are

The user base is evenly split between men and women across every age bracket.
The largest single group is 55 and over, with more than 35,000 users, which
makes it the most frequently underestimated segment in this kind of business.
Age based segmentation here is an opportunity, not a formality.

### How orders evolved

Total orders grow sharply from 2023 onward. Shipped and Complete dominate the
mix, which speaks well of fulfillment, but Cancelled and Returned grow alongside
volume rather than shrinking: friction is scaling with the business. Processing
stays stable, though it is the status to watch for bottlenecks.

### Inventory against sales

In every product category, stock exceeds units sold, with the widest gaps in
Intimates, Jeans and Tops. Best sellers concentrate in men's apparel and
accessories, led by Carhartt, Calvin Klein, Volcom and Ed Hardy.

## Recommendations

- Shift part of the paid budget toward SEO, where organic traffic underperforms
  relative to market size.
- Build a dedicated campaign for the 55+ bracket instead of treating it as
  residual.
- Investigate the growth in cancellations and returns starting from product
  descriptions and post purchase support, before touching logistics.
- Clear slow moving stock in the three categories with the largest overhang, and
  give best sellers permanent placement across homepage, email and social.

## Limitations

theLook is a synthetic dataset, so figures are directional rather than real
market data. The stock versus sales gap in particular is likely an artifact of
how the inventory table is generated, and would need validation against real
replenishment data before driving any purchasing decision.

Francesco Capitelli · Data Analyst · [LinkedIn](https://www.linkedin.com/in/francescocapitelli)
