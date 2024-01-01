# Contributing

There are two ways to contribute to this project:

## Using the form
You can upload your logos directly to the online form here: https://airtable.com/shrgqJLC3K14WeDWI. This usually takes about 24 hours to be reviewed and merged.

## Sending in a pull request
Another way to contribute is to directly send in a pull request. Here are some guidelines for this:

1. Ensure your logos have been properly optimised with tools like:
    [SVGOMG](https://jakearchibald.github.io/svgomg/) &
    [Squoosh](https://squoosh.app/) **(OxiPNG works well)**. Kindly ensure your file sizes are as small as possible. Also, your SVG file should be text-only and not contain any bitmaps.

2. Add a folder to **logos** named after your company. In this folder, put the svg and png versions of your logo. The files should have the same name as the folder and should be lowercase. If your company name has multiple words, kindly separate them with an underscore.

### Folder Structure
```
company_name
| company_name.png
| company_name.svg
```

3. In **[logos.json](https://github.com/aimen08/algerialogos/blob/master/logos.json)**, add a `JSON` entry for your company

### JSON Object
```
{
  "title": "Company Name",
  "filename": "company_name",
  "url": "https://company_url.com",
  "category": ["Category"]
}
```
**Example**
```
{
  "title": "Ooredoo",
  "filename": "ooredoo",
  "url": "https://www.ooredoo.dz/",
  "category": ["ICT","Telecommunication"]
}
```

4. If your company category is not reflected in categories section *below*, feel free to use a new category.
If you do so, kindly edit this file; adding the newly used category (**[/contributing.md](https://github.com/aimen08/algerialogos/blob/master/contributing.md)**) in your PR as well.
**NB:** Your jsonObject category can also be a combined form 2 or more categories in this form:  **e.g.**
```
"category": ["NGO", "Ecommerce"] or
"category": ["NGO", "Ecommerce", "Marketplace"] or
"category": ["NGO"]
```

5. Make sure your company URL has the `http://` or `https://` prefix or it will be rendered as invalid (this is to prevent some quirks in link redirection).
**NB:** By default, all empty or invalid urls will be linked to google search rather than the official website.
```
"url": "https://ooredoo.com" or
"url": "https://www.ooredoo.com"
not
"url": "ooredoo.com" or
"url": "www.ooredoo.com"
```

### Categories
```
* Banking
* Financial Services
* Branding
* Construction
* Coworking
* CRM
* Virtual Office
* Cryptocurrency
* Ecommerce
* Marketplace
* NGO
* EdTech
* FMCG
* Conglomerate
* Foundation
* Gaming
* Sports
* Government Agency
* Health
* Media
* Entertainment
* Newspaper
* Blog
* Petroleum and Gas
* Product Design
* Real Estate
* Restaurant
* Software
* ICT
* Telecommunication
* ISP
* Transportation
* Agritech
* Publishing
* Web Host
* Domain Registrar
* Local Search
* Business Ratings and Reviews
* Online Food Delivery
* Event Management
* PropTech
* Staffing and Recruiting
* Energy
* Electronics
* Pharmaceutical industry
* Open-source software
```

**NOTE**: _Pull requests are usually reviewed within 24 hours. Once your pull request is merged, you should see your logo on the site a few minutes after._