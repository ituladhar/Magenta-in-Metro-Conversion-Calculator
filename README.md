🟣 Magenta in Metro Compensation Calculator

This document provides technical and functional details for the Magenta in Metro (MiM) Compensation Calculator, an interactive tool designed for T-Mobile/Metro dealers. It allows for the real-time estimation of potential earnings by adjusting critical performance drivers within the MiM BAN Conversion program.

✨ Key Features & Benefits

The calculator is built as a single-file application for maximum accessibility and ease of deployment:

Real-Time Analytics: Instantly calculates total compensation, providing immediate feedback on changes to conversion rates or eligibility.

Professional Branding: Utilizes T-Mobile's Magenta for corporate theme alignment and prominent Green indicators for visual representation of profit and earnings.

Fully Responsive Design: Ensures an optimal viewing and interactive experience across all devices, from mobile phones to desktop monitors.

Strategic Opportunity Analysis: Benchmarks compensation potential against key performance targets (10%, 15%, 20% conversion).

Self-Contained Architecture: The entire application resides within a single index.html file, simplifying hosting and embedding.

⚙️ Financial Model: Core Calculation Logic

The compensation model is based on a fixed sequence of calculations using the inputs provided by the user.

BAN Conversions:

$$\text{BAN Conversions} = \text{Total MiM Eligibility} \times \frac{\text{Current Eligible BAN Conversion \%}}{100}$$

Lines Activated:

$$\text{Lines Activated} = \text{BAN Conversions} \times \text{Avg. MiM Conv. per migrated account}$$

Activation Comp $ Earned:

$$\text{Activation Comp \$ Earned} = \text{Lines Activated} \times \text{Rate Plan Value} \times \frac{\text{Standard Dealer Compensation}}{100}$$

Residual $ Amount:

$$\text{Residual \$ Amount} = \text{Activation Comp \$ Earned} \times \text{Empirical Residual Factor}$$

Total Compensation:

$$\text{Total Compensation} = \text{Activation Comp \$ Earned} + \text{Residual \$ Amount}$$

Note on Residual Factor: The Residual calculation relies on a fixed empirical factor (0.55200378). This value was derived from the proportional relationship between the Activation Comp and Residual values in the source spreadsheet data, ensuring the calculation accurately reflects the original model.

🚀 Deployment Methods

Since the application is a single index.html file, it can be hosted using various standard web services.

Option 1: GitHub Pages (Recommended for Hosting)

Ensure the file is explicitly named index.html.

Upload index.html to the root directory of your GitHub repository.

Navigate to Settings > Pages and configure the source to the main branch (or master) and the folder to / (root).

The application will be live at a URL such as yourusername.github.io/repository-name/.

Option 2: Embedding via Google Sites

Copy the entire content of the index.html file.

In the Google Site editor, use the Insert > Embed > Embed code feature.

Paste the HTML code and adjust the frame dimensions to ensure full visibility.

⚠️ Important Disclaimer

This tool provides a model-based estimate of potential compensation and is intended solely for informational and planning purposes. Actual earnings may vary and are always subject to final corporate audit, official compensation plan documentation, and policy changes. It does not constitute a guarantee of future income
