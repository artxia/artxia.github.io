---
layout: markdown_page
title: "Procurement - Purchase Order Process"
---

## On this page
{:.no_toc}

- TOC
{:toc}  

## Purchase Order Process

Once a Vendor issue has completed the [Procure to Pay Process](https://about.gitlab.com/handbook/finance/procure-to-pay), a Purchase Order is created in Netsuite. Before the Purchase Order can be completed, the vendor must self register/setup within Tipalti. Any delay in the Vendor Setup process will delay payment to the Vendor. Refer to [Vendor Master Management](https://about.gitlab.com/handbook/finance/accounting/#3-vendor-master-management) for the Vendor set up process.

To create a Purchase Order:

1. Login to Netsuite
1. Under the "Vendors" tab, follow the menu path:
    1. Vendors &rarr; Purchases &rarr; Enter Purchase Orders &rarr; List
1. In the "Purchase Orders" screen, select New Transaction
	1. Primary Information
		* Custom Form &rarr; This field should auto-populate with "Custom Purchase Order". 
		* Date &rarr; This field should auto-populate to the current date. 
			* If the date the Purchase Order is being completed is different from the date the contract is signed, update this field to reflect the date the contract is signed/executed.
		* Vendor # &rarr; This is an optional field and can be left blank.
		* PO # &rarr; "To Be Generated" should be displayed in this field with NO option to update.
		* Vendor &rarr; This is a drop down field. Select the Vendor. 
			* The Vendor should already be set up prior to creating a new PO. If the Vendor has not been set up, please refer to **[Vendor Master Management](https://about.gitlab.com/handbook/finance/accounting/#3-vendor-master-management)**
		* Memo &rarr; Copy and paste the Finance issue URL into this field. 
		* Supervisor Approval &rarr; Leave this box unchecked. **All approvals should already be obtained and tracked in the Finance Issue.**
		* Estimated Start Date &rarr; Date in this field should reflect the date the contract/services will begin.
		* Estimated End Date &rarr; Date in this field should reflect the date the contract/services will expire.
		* Receive By &rarr; This field is optional and can be left blank.
	1. Classification
		* Subsidiary &rarr; Select the applicable Subsidiary.
		* Department &rarr; Select applicable department.
		* Class &rarr;  This is an optional field but is required to be completed by the Marketing Team. Enter the Campaign Finance Tag.
	1. Intercompany Management
		* Paired Intercompany Transaction &rarr; This field is optional and should be left blank.
		* Currency &rarr; Default should be "US Dollar".
		* JE Support: Google Drive Link &rarr; This field is optional and should be left blank.
		* Requestor Name &rarr; This field should auto-populate to the team member's name that is creating/entering the Purchase Order.
		* Created From &rarr; This field is optional and can be left blank.
	1. Items
		* Exchange Rate &rarr; This field should auto-populate with the value "1.00".
		* Expenses &rarr; This section will document the product/service.
			* Category &rarr; Select the applicable expense.
			* Account &rarr; Field should auto-populate based off of "Category" selection.
			* Amount &rarr; Enter the full contracted dollar amount.
			* Memo &rarr; Optional Field
			* Department &rarr; Select applicable department.
			* Class &rarr;  This is an optional field but is required to be completed by the Marketing Team. Enter the Campaign Finance Tag.
			* Customer &rarr; Optional Field
			* Billable &rarr; Optional Field
			* Receipt URL &rarr; Optional Field
			* Related Asset &rarr; Optional Field
			* **Select "Add"**
			* If no additional items need to be added, Select the "Billing" tab. If additional items need to be added, you may add them now by manually entering in the new information or selecting "Copy Previous".
	1. Billing
		* All fields in this section are marked as optional fields but **will be required to be completed**. Information entered in this section will be displayed on the Purchase Order under the Vendor Information section. If this is left blank, Vendor information will not be displayed on the Purchase Order.
		* Vendor Select &rarr; Select from the applicable list.
			* Select New to enter a new address for this transaction and save it to the associated vendor record.
			* Select Custom to enter a new address to use for this transaction only. It is not saved with the associated vendor record.
			* Select the Edit icon to modify an existing vendor address. The Edit icon will be to the right of the Vendor Selection drop down field.
		* Vendor &rarr; This field will auto-populate with the Vendor Information entered during the "Vendor Select" process.
		* Terms &rarr; Select from the applicable list.
		* Incoterm &rarr; This field can be left blank.
	1. Relationships
		* Contact &rarr; Enter vendor contact name in this field.
		* Job Title &rarr; Vendor contact job title
		* Email &rarr; Vendor contact email.
		* Main Phone &rarr; Vendor contact phone number.
		* Subsidairy &rarr; Select from the applicable list.
		* Role &rarr; Selecl from the applicable list.
		* **Select "Add"**
	1. Communication
		* Messages
			* Select checkbox "To be E-Mailed" and populate with vendor email address.
			* Vendor Message &rarr; Information entered in this field will be printed on the Purchase Order.
1. Once all information has been entered, select "Save".
1. Screen will refresh and a message banner at the top of the screen will be displayed with Transaction save confirmation. You will see a message stating "Pending Receipt".
1. Select "Receive" to complete the Purchase Order Process. 
