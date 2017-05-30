# PayItMonthly Simple Integration

PayItMonthly enables your business to offer your customer finance. 

This guide shows you how to embed our simple integration within your website.

## Support

If you need to contact us for any reason you can email us at [support@payitmonthly.uk](mailto:support@payitmonthly.uk) or call us on 0333 212 3914.

## Getting Started

You need to opened a live account at [PayItMonthly](https://payitmonthly.uk). Once your account is live you can request your API key by emailing [support@payitmonthly.uk](mailto:support@payitmonthly.uk).

## HTML Form Based Application

```markdown
<form action="https://payitmonthly.uk//" method="post"> 
    <input type="hidden" name="identification_key" value="adfwt2894ahgBUDSFOHE8we9"/> 
    <input type="hidden" name="goods_description" value="Photos - CD - Gold Package"/> 
    <input type="hidden" name="goods_price" value="60000"/> 
    <input type="hidden" name="finance_deposit_total" value="6000"/> 
    <input type="hidden" name="test_or_live" value="test"/>
    <input type="hidden" name="finance_max_duration" value="8"/>
    <input type="hidden" name="finance_number_of_instalments" value="10"/>
    <input type="hidden" name="finance_first_payment_date" value="20170720"/>
    <input type="submit" value="Buy on Finance"/> 
</form>

```
## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/payitmonthly/integration/edit/master/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/payitmonthly/integration/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
