# tds-project-1

   Project Overview
1. Data Scraping Process

This project collected GitHub user data from Basel with the following process:

    Authentication: Used a GitHub Personal Access Token (PAT) in request headers for authorization and to avoid rate limits.
    Targeted GitHub users located in Basel with more than 10 followers by using the query location:Delhi+followers:>100. Results were limited to 100 users per page (GitHub’s max).    Pagination: To retrieve all qualifying users, the script fetched multiple pages until the API returned no more results.

    Detailed User Information: Additional API requests provided in-depth details about each user, including name, company, and public repositories. For each repository, key details like stars, language, and presence of projects or wikis were collected.
    Data Cleaning: Standardized company names (e.g., removing “@” symbols, converting to uppercase) and handled missing data (e.g., for emails and company names).
    CSV Output: Data was saved into two structured CSV files: users.csv (for user details) and repositories.csv (for repositories).

2. Interesting Findings from Data Analysis

The analysis surfaced some interesting insights about GitHub users in Basel:
    Diverse Industry Representation: Contrary to expectations, many users in Basel come from industries outside traditional tech, such as healthcare, pharmaceuticals, and research. This aligns with Basel's strong focus on life sciences and biotech.
    Data Science and Automation Focus: A significant number of repositories were centered on data science and automation rather than general software development, reflecting a demand for data-driven applications, likely due to the scientific and research-oriented community in Basel.

3. Actionable Recommendations for Developers

Based on these insights, here are some recommendations for developers looking to engage with Basel's GitHub user base:

    Develop Tools for Scientific Computing: Libraries and applications focused on data visualization, statistical analysis, or biotech-specific tools could see high interest and adoption among Basel-based users.    Open-Source Contributions: Contributing to or developing open-source projects in scientific computing, data analysis, or automation can help build a strong reputation within Basel's biotech and research sectors.    Industry-Specific Solutions: Basel users likely value data privacy and regulatory compliance, especially for applications in healthcare and life sciences. Tailoring applications to address these needs (e.g., data security, automated workflows) could enhance engagement and trust.
