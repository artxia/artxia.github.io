---
layout: handbook-page-toc
title: "Merchandise Workflow"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Merchandise Overview

Community Relations manages the merchandise store. This includes:
- adding and removing items to and from the store,
- fulfilling orders,
- maintaining inventory levels and
- responding to store support requests

### Accounts overview

Shopify is our storefront vendor
- URL: https://shopify.com (use gitlab.myshopify.com if prompted for the store address)
- Login: see 1Password secure note for details
- Account permissions: [Staff account](https://help.shopify.com/en/manual/your-account/staff-accounts) is required to access the admin. Staff accounts can only be created by the [store owner](https://help.shopify.com/en/manual/your-account)
- Note: Community Advocates use a shared account, as the number of staff accounts for our [current subscription](https://www.shopify.com/pricing) is limited to 5.

Printfection is our main inventory vendor for general merchandise
- URL: https://www.printfection.com/
- Account permissions: `print`, `manage`, `admin` 
- Login: use Community Relations 1Password credential from the marketing vault.
- Note: we are currently using a shared account, but we should migrate to individual accounts for each Community Advocate

Stickermule is our main inventory vendor for stickers
- URL: https://www.stickermule.com
- Login: see 1Password secure note for details

### Shopify and Printfection

When a customer visits the [GitLab Store](https://shop.gitlab.com/), they see available products on the front end Shopify store. Advocates manage customer orders using Shopify's backend. Orders are processed and items are shipped through Printfection, which GitLab uses as the store warehouse.

### Shopify/Printfection Zapier Integration

All the orders received via [shop.gitlab.com](https://shop.gitlab.com/) are automatically forwarded from Shopify to Printfection via the Printfection-Shopify Zapier integration. On Printfection we manually process the orders and fulfill the shipments. You can always check the status of the orders in the collection tab in Printfection.

### Choosing a Vendor

Most swag items are purchased through Printfection. 

As a general rule, consider using [Stickermule](https://www.stickermule.com) for sending stickers, since the Printfection inventory is limited. If Stickermule doesn't work for you, then use Printfection instead.

If the merch shipment includes:
* only stickers, always use Stickermule
* a small number of items (depending on Printfection inventory), use Printfection
* a large amount of stickers and other merch, consider using both Stickermule and Printfection

<i class="fas fa-hand-point-right" aria-hidden="true" style="color: rgb(138, 109, 59)
;"></i> Always check the Printfection inventory and item availability before sending.
{: .alert .alert-warning}

Examples of events where you might order stickers in large quantities from StickMule include:
* Hackathons
* Conferences
* MeetUps

### Ordering on StickerMule

StickerMule is the preferred Vendor for orders that include only stickers, or orders that include a large number of stickers. StickerMule orders for the Community team should be placed with the Corporate Marketing credit card.

1. Log in to StickerMule
2. Navigate to the 'Reorder' tab
3. Select the sticker you'd like to order based on stickers created from previous orders. New stickers can be created, but if possible, it is faster to reorder an existing sticker.
4. Exisiting stickers vary in size, but most are between 2.64"x3"
5. Stickers must be orders in batches of 10
6. Enter sticker quantity and process Stickermule order.
7. Send orders to the wider community member, Meetup organizer, customer, or Printfection warehouse. The Printfection warehouse address is: 700 W 48th Ave, Denver, CO 80216
8. When adding shipping information, add the project title or finance tag to the `Company` line so that orders can be tracked.
9. If shipping to Printfection, follow steps in Printfection to create a 'Send' inventory order.


## Daily Merchandise Workflow

One of the main community advocate tasks is to fulfill all the GitLab swag orders.

Advocates should check for new orders daily as the orders should be fulfilled and shipped in a timely manner. In order to process these orders you'll have to fulfill them both in Shopify and Printfection.

[Video tutorial](https://drive.google.com/file/d/16pcdtfwbNye0SmtX20QOhqwP0TYbijVG/view?usp=sharing) available for GitLab team members.

### Where to Find Merchandise Notifications
* Make sure you regularly check the #swag channel and the Merchandise view in the Zendesk.
* If the recipient is  a contributor, user or customer make sure you reach out to the recipient via <community@gitlab.com>:
  * Thank them for their work/support
  * Gather the missing info needed for fulfilling the swag dropship if needed
* Fulfill the shipment in Printfection:

<i class="fas fa-hand-point-right" aria-hidden="true" style="color: rgb(138, 109, 59);"></i> Please bear in mind the [list of countries we do not do business in](/handbook/sales/#export-control-classification-and-countries-we-do-not-do-business-in).
{: .alert .alert-warning}

### Shopify

GitLab uses Shopify as a customer facing online store and backend order fulfillment. Fulfilling orders in Shopify serves to send the actual notification that an order has been processed, including the invoice for the customer.

1. Login to Shopify
2. Go to the orders page
3. Make sure to check all the new orders highlighted with the yellow Unfulfilled tag.
4. Before fulfilling orders, begin the Printfection order fulfillment process. It is important to confirm that Shopify and Printfection orders are the same before fulfilling.
5. Click on actions > fulfill selected orders
6. Make sure that the default "send a notification" option is selected and press the fulfill button

That's all, the customers should receive their confirmations automatically.

### Printfection

GitLab uses Printfection as both a vendor and a warehouse. Fulfilling orders in Printfection means that Prinfection will pack and ship items to the customer.

1. Login to Printfection
2. Navigate to the Collection Orders and choose "Shopify Store Orders."
3. Go to the Manage tab
4. Make sure that all unfulfilled orders from Shopify are shown in Printfection and that everything is okay.
5. If an order appears in Shopify but not in Printfection, follow the workflow to manually add an order
6. Press the "Place Orders"

That's all, Printfection will handle the rest. 

Note: Printfection also sends the email confirmation to the customer.

### Zendesk
1. Check the Merchandise ticket view in Zendesk for any emails sent to merch@gitlab.com
2. For updates sent automatically from Printfection, apply the 'Printfection Update' macro to solve the ticket.
3. For merchandise questions and order follow up emails, follow processes outlined below.

### Manually Add Orders to Printfection

If orders unfulfilled orders appear in Shopify but are not in Printfection, you might need to manually add the order to Printfection before fulfilling the order.

Before manually adding orders, use the search tool in Printfection to check for orders that are unfulfilled in Shopify. Sometimes, a user will fulfill orders in Printfection without checking Shopify. If you find that an order has already been fulfilled in Printfection, simply fulfill the order in Shopify.

If you cannot locate the order in Printfection, you'll need to manually add the order.

1. Login to Printfection
2. Navigate to the Collection Orders and choose "Shopify Store Orders"
3. Go to the Manage tab
4. Click the "Add Order" button
5. Click the "Add an Item" button to add items from the GitLab Shopify store to the order. Use the original order from Shopify as a guide to choose the correct product and size
6. Use the original order from Shopify to copy all relevant customer information into the Printfection order. Be sure to include name, shipping address, and email address
7. Click the "Save Order" button then the "Place Order" button
8. Complete the workflow for fulfilling the order in Shopify


## Inventory Management

### Manual Check/Update of Inventory

Sometimes, the Shopify/Printfection integration does not successfully update inventory amounts in the Shopify store. 

It is important for community advocates to compare Shopify and Printfection inventories approx. 1x per week to avoid out of stock orders from being processed. This is a high priority for products with low inventory.

#### Check Printfection Inventory
1. Log into Printfection
2. Click on Inventory
3. On the Inventory page, click on Inventory Levels
4. The data colummn titled 'Physically Available' is the most important data point. This represents the number of that item that currently available in the warehouse 

#### Check Shopify Inventory
1. Log into Shopify
2. Click on Products
3. Click on individual items to review their inventory details
4. Compare inventory numbers in Shopify with Physically Available information in Printfection. Update accordingly in Shopify

### Replenish Printfection Inventory

Community Advocates should watch inventory levels for products in Printfection and order more inventory when inventory is low. Replenish orders typically take 2-3 weeks until items are physically available in the warehouse.

1. Log into Printfection
2. Click on Inventory
3. On the Inventory page, click on Replenish Inventory
4. Click the green 'Replenish Inventory' button
5. Choose the 'Print' tag option
6. Give a name to your print order that describe the inventory you are ordering
7. Click the 'Start Replenish Order' button
8. Add Printfection items to the order. Specify the quantity for each item. Notice that some items have a minimum order number. Be mindful of total cost of items and try to order items in bulk, as the price per item decreases for larger quantity orders
9. When you've completed your replenish order, click the 'Buy Items' button

### Send Items to Printfection Warehouse

Printfection does not produce all items we sell in the store. To ship items from another vendor to Printfection, you must create a 'Send' inventory order. 
1. Log into Printfection
2. Click on Inventory
3. On the Inventory pate, click on Replenish Inventory
4. Click on the green 'Replenish Inventory button'
5. Choose the 'Send' tag option
6. Enter product details, quantity, and shipping confirmation, then submit the order’

### Creating and Ordering New Swag Items

The Marketing team aims to create swag that is "small batch, limited edition and themed for the community to collect." To uphold this value, swag store items are frequently swapped out and replenished with new and different swag. Follow these steps to create new swag items for the Shopify store.

1. First, review the [Corporate Marketing Swag handbook page](/handbook/marketing/corporate-marketing/#swag). Keep these swag requirements in mind while planning and brainstorming new items.
2. Consider brainstorming with other GitLabbers in the #swag channel. Post a poll or a open an issue and ask for swag requests. See this [issue](https://gitlab.com/gitlab-com/marketing/community-relations/community-advocacy/general/issues/56) for an example.
3. View the [Printfection Catalog](https://www.printfection.com/swag/) for item inspiration.
4. If you cannot find and item you like in Printfection, contact the Nadel vendor representative with an item request. Nadel can source items for you and will reply with an item mock up.
5. After deciding on a product, collect the following information: Item Cost, Size/Dimensions, Weight, and Color Options
6. Open an issue in the [Corporate Marking Project](https://www.printfection.com/swag/) using the `design-request-general` template. All new swag requests must go through Corporate Marketing for design/artwork consistancy.

### Adding Products to Shopify

1. Gather item inventory data from Printfection and Product Vendor. You will need: product description, title, weight, high resolution image, SKU, and Size IDs (if item has variants). Most information can be found direction in Printfection within each item view. If items are missing, follow up with the product vendor via email.
1. Log in to Shopify
1. Open the products page
   - Click the Add Product button
   - Fill out information about the item. Include the title, size description, weight, and size variants.
   - Include the SKU and Size ID numbers, found in Printfection.
   - Upload an image for the product. Be sure it is high resolution. Shopify suggests using images with 2048 x 2048 pixel resolution for square product photos.
   - Fill out the price for the item.
   - Select "Shopify tracks this product's inventory"
   - Check the product availability and select Online Store.
   - Before saving the product, please check search engine listing preview
   - After saving the new item, navigate to the Collections tab and select the 'catalog' collection
   - Add the new item to the catalog.
   - In order for the new item to show on the Shopify store, you may need to edit the UI of the Shopify store. To do this, choose the Online Store tab. Naviagate to Themes -> Customize -> Home Page. Edit the number of rows and products per row to include all catalog items. A maximum of 25 items can appear on the home page at 1 time.

<i class="fas fa-info-circle" aria-hidden="true" style="color: rgb(49, 112, 143)
;"></i> For more information, see this [official guide](https://help.shopify.com/en/manual/products/add-update-products)
{: .alert .alert-info}

### Removing Products from Shopify

1. Log in to Shopify
1. Open the Products page
   - Click on the product you want to remove
   - Scroll to the bottom of the page where you can find the delete button

<i class="fas fa-info-circle" aria-hidden="true" style="color: rgb(49, 112, 143)
;"></i> For more information, see this [official guide](http://shopifynation.com/shopify-tutorials/delete-products-variants-shopify/)
{: .alert .alert-info}


## Additional Order Workflows

### Printfection fulfillment notifications

The updates about the orders are sent to both <merch@gitlab.com> and the customer's email address. You can find those messages in the `Merchandise` view on [GitLab Community Zendesk instance](https://gitlab-community.zendesk.com/).

### Canceling any external order on Shopify and Printfection

You can always cancel the pending/processing orders. All the orders including the orders via Shopify Collections using Discount Codes can be canceled.

1. From your Printfection home page go to the **Shopify store orders** collection.
2. Under the **Manage** tab, search for the order you want to cancel.
3. Click **Delete order** button.
4. You are done. The order won't be fulfilled by Printfection

Please note that you should always change the status of the orders in Shopify as well.

1. From your Shopify admin page go to the **Orders** page
2. Click on the order you want to change
3. Press **More Actions** button in order to see the drop menu options
4. Select **Cancel order** option

### Tracking IDs

The Tracking ID is usually assigned by Printfection 2-3 days after the order is received. Sometimes, users may request their Tracking ID.

Please follow these steps if the user requests the Tracking ID:
1. Look for the requester's **name/email**
2. Go to the Printfection **Reports** page
3. Search for the order using the name/email
4. Copy the **Tracking ID**
5. Confirm that order's details match the requester. You can double check this via Shopify:
    * Search for the same order/person in Shopify
    * Compare if the **items**, **full name**, **email** and the **dates** are correct
6. Email the **Tracking ID** or the full **Tracking Link** to the requester
    * You can always open the full **Tracking Link** by clicking on the **Tracking ID**.
7. (Optional step) Assign the **Tracking ID** to the requester's order in Shopify:
    * Find the order in Shopify
    * If you already fulfilled the order in Shopify, click **Add tracking** button and paste the ID.
    * If the order is unfulfilled in Shopify, mark it as **fulfilled** and then add the **Tracking ID**

### Sending merch via Printfection 

1. Go to any collection on Prinfection
2. Click on **Manage** tab
3. Press the **Add order** button
4. Pick the items and enter the **quantity**
5. Important: click **Save order** button
6. Input the shipping details
7. Imporant: click **Save order** button
8. You are ready to click the **Place the order** button

### Creating the discount codes

In order to create a coupon code on Shopify, please check out this [video tutorial](https://drive.google.com/file/d/1h9ZJgktR2iGxJqz7Fqy9FqMjVtF19YJ9/view?usp=sharing).

### Creating Giveaway Kits
Giveaway kits in Printfection are an efficient way to create bundles of swag to send to community members because they allow you to set limits on item totals. For example, these could be utilized for Meetup organizers to place orders for a giveaway kit of tshirts, stickers, and notebooks.

1. In Printfection, start by creating a giveaway kit with your desired items. For details, follow [the documentation to start a new kit](https://help.printfection.com/hc/en-us/articles/360006335613-How-to-start-a-new-kit).
2. After creating the kit, use [the documentation to create a giveaway campaign](https://help.printfection.com/hc/en-us/articles/360026589734-Using-kits-in-Giveaway-campaigns).
3. Kits can be added to giveaway campaigns just like a regular swag item, as defined in the documentation above.
4. When your giveaway kit is created, you can generate order links in Printfection. Send these links to the desired community member so they can self place their orders.
5. Note that whatever you name your giveaway campaign will be visable by the customer, so be sure to make it clear and accurate.
6. Important Note: Each giveaway kit link will redeem 1 single kit. If a customer needs more swag, consider sending them multiple giveaway kit links.

### Creating External Order Links
External order links are an efficient way for GitLab team members to place swag orders. For example, the Sales team uses an external order link for Sales employees to send merchandise to customers and prospects.

External order links can only be used by users with the @gitlab.com domain, so they are not an efficient tool for wider community orders.

1. First, create a new collection campaign. Navigate through Campaigns -> Collections -> + Collection Campaign to create a new one.
2. Name your campaign and click the blue 'Create Campaign' button.
3. Add items to your campaign by clicking the 'Items' tab and selecting swag from the inventory. When adding an item with variable sizes, choose any size as a place holder. When customers access the order link, they can select/edit sizes and qualities.
4. Next, on the 'Overview' tab, scroll down to the section titled 'External Orders'. Toggle this setting to 'On'.
5. You can make additional edits to the External Order form by clicking the 'Settings' tab. Here you can make changes to the UI of the external order link.
6. In the 'Overview' tab, you'll see the external order link you can send to GitLab employees where they can place their order. You'll have to manually approve orders in Printfection in order for them to be fulfilled.

### Refunding Orders

Sometimes orders need to be refunded to the customer. An example of this could be if a customer places an order for an item that is out of stock. Refunds are processed through Shopify.

1. Find the order in Shopify
2. Check Paid notes to see the total amount paid by the customer
3. Click 'Refund'
4. Add a reason for the refund. This is an internal note
5. Add the total amount for refund
6. Click the 'Refund' button to process the refund to the user
7. Find the user email address on the order and send them an email via the merch@gitlab.com email address. Explain the reason for the refund and include a link to a discount code to be used on a new order.

### Monthly report sharing

The GitLab accounting team has access to Shopify and Printfection. Accounting manager Kim S. runs monthly reports for the swag store.

Previous month reports can be viewed in this [google folder](https://drive.google.com/drive/folders/1uCUfakIR7E188hPg14pBcLZWsoz6KT7O) accessible only by GitLab team members.

If an advocate needs more information about how to access reports in Shopify and Printfection, please follow the steps in this [video tutorial](https://drive.google.com/file/d/1TiVxM9an0SIFrqp7ESj4QiqIj0ekAZ3F/view?usp=sharing).

### Delayed and lost merchandise shipments

From time to time it may happen that the package never arrives to the customers. Customers usually complain via <merch@gitlab.com>, however, keep an eye on Twitter, the #swag Slack channel and other related threads.

Please check if the package is still in transport using the tracking ID and reach out to the customer with brief details.

If the package has been in transport over 2-3 weeks, apologize, refund the order, and create a 20% off discount code for future orders:
1. Login to Shopify.
2. Search the order by name/email/orderID.
3. Select the order.
4. Select the "Refund items" option.
5. On the right part of the page, you have the fields to enter the custom value and reason for a refund.
6. If you are not sure how to calculate the 20%, multiply 0.2 with the whole amount and that's the exact value.
7. Use "Reason for refund" field and write the appropriate message explaining that we are refunding 20% of the whole amount due to delayed shipping and press the Refund button.
8. Don't forget to apologize to the customer using the original thread (e.g. respond via the original Zendesk ticket) and offer any other assistance if needed.

If the customer complains that the package never arrived and the package status is "completed" or "delivered", consider the following options:
1. Reach out to the vendor (<support@printfection.com> or <help@stickermule.com>) and ask if they have information about that specific order.
2. If the package has been returned or lost, consider asking them to resend it.
3. If the vendor doesn't resend the package, do it manually asap.
4. Always consider refunding the whole order amount to the customer.
5. Since we care about our community and customers, feel free to include extra item/s of your choice, create a coupon code for an apology or any other idea. In this case, the main goal is to make the customer happy.
6. Don't forget to coordinate everything with the customer (use <merch@gitlab.com> for conversation), apologize and find out if there's any other thing we could do for them.

### Customs Issues for Shipments outside of the USA

Since all swag in the store ships from our warehouse in Denver, CO, USA, customers outside of the US may have issues with customs tax payments upon delivery of their package.

The Advocates team is working on the possibiliy of creating a customs statement for swag shipments to avoid these costs. Updates can be followed in [this issue](https://gitlab.com/gitlab-com/marketing/community-relations/merchandise/general/issues/12).

Until the customs statement is created, the following strategies can be used to avoid customers paying the tax.

1. At checkout in the Shopify store, customers can choose Expedited or Priority Shipping and email merch@gitlab.com for reimbursement of shipping costs.
2. If a customer reports their swag cannot be delivered due to a customs issue, advcoates can place a new order via Printfection and choose the 'Ship By Date' option to insure delivery.
3. For large orders of swag, or orders with multiple items, customers and advocates can break up the order into multiple, smaller orders. This may prevent packages from being stopped for customs tax.

## Swag Giveaways and Internal Requests

### Collections 

Printfection's Collection campaign is a way to easily collect orders, review them, and then place them all at once. You can manually key-in orders, import orders from a CSV file, or allow other parties to place orders through a hosted landing page.

#### Create a new Collection campaign

1. Go to Campaigns tab then click Collections 
2. Click the **+COLLECTION CAMPAIGN** button. 
3. Enter the name,
4. Select the option that turns on External Ordering (this option will provide you a link that allows users to place orders for this campaign).
5. Press **CREATE CAMPAIGN** button.
6. Go to the **Items** tab in the navigation menu.
7. Click **Add Items to Campaign** and simply choose the items you want to offer in your Collection.
8. Go to **Settings** in the navigation menu and update the GitLab branding (see the existing givaway settings). You'll also need to specify a payment method on this page.
9. Turn the campaign from **Paused** to **Running** in the top right navigation menu. And that's it, you're ready to give some swag!

Last, but not least, you'll want to review the orders from the Manage page within your Collection campaign. Here you can change, update, or remove orders. Review your totals, fulfillment cost, and other details.  When you're ready hit Place Orders and place them all at once!

### Giveaways

Printfection has the giveaway campaigns which allow us to send a link to our customers and let Printfection handle the rest.

The giveaway campaign works like this:  

1. Choose your swag offerings & brand your redemption page
2. Send out giveaway links
3. Customers enter their name and address
4. **Manually** fulfill the order in Printfection.

### Create a new Giveaway campaign
 
1. Go to Campaigns tab then click Giveaways 
2. Click the **+ GIVEAWAY CAMPAIGN** button. 
3. Enter the name and press **CREATE CAMPAIGN** button.
4. Go to the **Items** tab in the navigation menu.
5. Click **Add Items to Campaign** and simply choose the items you want to offer in your Giveaway.
6. Click the **Manage** in the navigation menu and choose how many initial links you want to giveaway (you can always add more later).
7. Go to **Settings** in the navigation menu and update the GitLab branding (see the existing givaway settings). You'll also need to specify a payment method on this page.
8. Turn the campaign from **Paused** to **Running** in the top right navigation menu. And that's it, you're ready to give some swag!

Note: Once a redemption is complete you will have the option to cancel it from the 'Recipients & Redemption' section at the bottom of the 'Overview' page. Just use the 'Cancel' button next to the order. This cancelation option is only available until the order is processed, you'll want to review orders same-day or earlier if you want to cancel them.

### Updating the contributors giveaway sheet 

We are sharing swag giveaway links to the community contributors. Advocates should replenish the links each quarter and update the with the new links [sheet](https://docs.google.com/spreadsheets/d/1kzK25SE9jPXx50Lw0W8jtm9u77Zr4w13FAg1gyD6Egk/edit#gid=1578711076).

Please check out this [video tutorial](https://drive.google.com/file/d/1uggqOMkywNbqoPBJjkjAAJAcGz-HQjZH/view?usp=sharing) no how to update the sheets or follow the steps bellow:

1. Login to Printfection.
2. Go to "Community Contributor" giveaway campaign.
3. Click on the Manage tab.
4. Generate new links.
5. Make sure to download the CSV file of the freshly created links only
6. Upload the csv file or copy/paste the new links into the [sheet](https://docs.google.com/spreadsheets/d/1kzK25SE9jPXx50Lw0W8jtm9u77Zr4w13FAg1gyD6Egk/edit#gid=1578711076)

### MVP Appreciation Gifts

Each 22nd of the month is a release day - every release we pick a Most Valuable Person and thank them for their contributions. We send them some GitLab swag as a thank you (e.g. a hoodie, socks, and a handmade tanuki). There's also the option of sending personalized swag - see [custom swag providers](#good-custom-swag-providers).

1. Determine MVP after merge window closes, see `#release-post` channel
1. Find MVP's contact information
  * An email address is usually stored in git commit data
  * A user might have email or twitter info on their profile
1. Congratulate the MVP via email, ask for their shipping address, as well as any other relevant information (e.g. shirt size)
1. Investigate the MVP's interests
  * If the MVP doesn't have a notable presence on social media, you may choose to ask them directly or send GitLab swag instead
1. Choose a suitable gift (up to 200$ USD)
1. Write a kind thank you message
1. Send the gift
  * The MVP should ideally have the gift 48h before the post goes live, though shipping to people outside the United States can take longer and usually won't make it in time
1. Verify shipment status
  * Make sure that it was sent
  * Make sure that it arrived
1. Mention the MVP gift in the release post
  * Make sure there's a picture of the gift in the release post if it's available

### Giveaway Requests from GitLab Teams
Community Advocates may be asked to support other teams at GitLab who are organizing a giveaway promotion. Use this list a guideline for collaborating with these requests.

* Assess inventory in the swag store to see if the current item quantity can support the giveaway.
* If the store is low on inventory, alert the organizing team that an order needs to be placed first, and to consider timeline for swag availability in the planning stages.
* Discuss where the budget for swag will be allocated from.
* In some cases, it makes sense for the team organizing the giveaway to create their own [Corporate Marketing issue](https://gitlab.com/gitlab-com/marketing/corporate-marketing/issues) to create new swag items. In this case, the advocate can provide support in ordering/shipping these items to the Printfection warehouse.
* Giveaways can be done either directly through Printfection or using the Shopify store discounts. Advocates can support the organizing team by either creating these giveaway campaigns or discount codes.

### Swag Requests

Please use this table to confirm you're using the correct order process for GitLab Swag:

| Swag Order Scenario | Order Process|
| --- | --- |
| You're speaking at an upcoming event and would like to bring GitLab swag | Follow the [Swag for Speaking at or Hosting GitLab events process](/handbook/marketing/community-relations/community-advocacy/workflows/merchandise-handling/#swag-for-speaking-at-or-hosting-gitlab-events) |
| You're hosting an event and you'd like to share GitLab swag | Follow the [Swag for Speaking at or Hosting GitLab events process](/handbook/marketing/community-relations/community-advocacy/workflows/merchandise-handling/#swag-for-speaking-at-or-hosting-gitlab-events) |
| You're ordering swag for a customer | Use the [Printfection Sales Swag](https://get.printfection.com/dcdzm/6508378270) link. This link is for GitLab internal use only and you must log in with your @gitlab.com address. If you are a new user enter your @gitLab.com address in the login page and follow the instructions to set up your account. Review the [Swag for Customer/Prospects](/handbook/marketing/corporate-marketing/#swag-for-customer-prospects) for guidelines on order sizes. |
| You want to recognize a wider community member for their contributions | Use the [Internal Community Contributions Swag process](/handbook/marketing/community-relations/community-advocacy/workflows/merchandise-handling/community-rewards-internal/) |

### Swag for Speaking at or Hosting GitLab Events

Gitlabbers can request a merch order for an event they are speaking at or hosting by emailing the request to <merch@gitlab.com>.

Please use the following email template when placing a merchandise request:

```markdown
Hello Merch Team,

I'd like to place the following GitLab merchandise order:

Reason for Order: 

Item Name: 
Size, if applicable: 
Quantity:


Name for the order:
Shipping Address:
Email Address:
Phone Number:


Regards,
YOUR_NAME
```

Notes: we recommend that you request merchandise at least 4 weeks in advance for us to be able to accommodate your request. However,
* If your request is urgent, please reach out to the swag expert and find out if the fast shipping option is available.
* Feel free to schedule a Zoom call with the swag expert to discuss, create and place the order.
* The swag expert should send the notification when the order is placed.
* Tracking IDs are available once the package is shipped which usually takes 1-2 days.
* In order to keep the orders transparent, please do not send requests via direct messages, but email <merch@gitlab.com>.
* the #swag Slack channel can be used to ask questions about swag or the order process.




