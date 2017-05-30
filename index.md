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

## Parameters

Name | Description | Required | Type | Validation
-----|-------------|----------|------|-----------
identification_key| Public API key | Yes | string	
test_or_live | This specifies which mode to operate the system in | Yes | string | 'test' or 'live'


goods_description	Description of the goods/service that the customer is purchasing. This will be shown on the customers agreement	Yes	string	
goods_price	Price of the goods/service that the customer is purchasing in pence before the deposit is taken. The value of finance required is calculated automaticly (goods_price - finance_deposit_total)	Yes	int	Positive integer
finance_deposit_total	Total deposit paid/to be paid by the customer in pence	Yes	int	Positive integer
finance_number_of_instalments	Number of instalments that the customer will pay - do not include the deposit as an instalment	No	int	Between 1-12
finance_max_duration	Maximum number of instalments/months that the customer can choose if you want it to be less than 12. This value is not used if the number of instalments is set	No	int	Between 1-12
finance_first_payment_date	The date of the first repayment that the customer will make. If this isn't set the customer will be able to choose the date that works best for them. Each subsequent instalment will be taken on the same date each month	No	ISO 8601	Minimum of 7 and maximum of 60 days in the future
customer_title	Customers title	No	string	Either 'Mr.', 'Mrs.', 'Miss.', 'Ms.' or 'Dr.'
customer_firstname	Customers firstname	No	string	
customer_middle_name	Customers middle name	No	string	
customer_surname	Customers surname	No	string	
customer_mobile	Customers mobile number	No	string	
customer_landline	Customers landline	No	string	
customer_email	Customers email address	No	string	
customer_address_line_1	House Number/Name	No	string	
customer_address_line_2	Street Address	No	string	
customer_address_line_3	Town	No	string	
customer_address_line_4	County	No	string	
customer_address_postcode	Postcode	No	string	



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
