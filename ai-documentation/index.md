# ReAccess AI Introduction

The AI Documentation is meant to help both the user and AI to build out an Excel file which is used to create a new ReAccess app.  If you want to use the UI no-code solution please use our App Builder platform.  Below are the steps to create and excel doucment which you can then import in ReAccess.

## Steps

1.  Create an importable Excel document that ReAccess can consume.  

    To do this you must first create an Excel document normally with the Application Name as the document name.

2.  Create twelve tabs within the Excel document labeled Application, Forms, Form Filters, Form Row Filters, Controls, Tabs, Dropdowns, Webhooks, Rules, Grids, Grid Columns, API Keys

3.  On the Application tab the document must contain the following columns and make them bold if possible.  Anything with an asterisk is required from the user.  Also, tags are seperated by semicolons.  If an icon is not provided, use "Home" as the default.  If a value is not provided for the columns "Call Webhook on Publish" or "User PowerBI Report as Home Page" use False as a default value when generatng the Excel document.

    Application Tab Columns:
    -   Name*
    -   HomePageContent
    -   Tags*
    -   Description*
    -   Icon*
    -   Report URL
    -   Call Webhook on Publish
    -   Webhook URL
    -   Authorization Type
    -   Key
    -   Value
    -   Add To
    -   User Name
    -   Password
    -   User PoweriI as Home Page
    -   Workspace ID
    -   Report ID
    -   Report with RLS?
    -   Roles
    -   Is Background Transparent?
    -   Show Border?
    -   Is Filter Visible?
    -   Is Filter Expanded?
    -   Is Page Navigation Visible?
    -   Height
    -   Width
    


4.  A form is synonymous to a page inside ReAccess.  It will house the data elements you wish to collect on which are called controls.  Here we will create the Form tab data elements.  On the Forms tab the document must contain the following columns and make them bold if possible.  Anything with an asterisk is required from the user.  Also, tags are seperated by semicolons.  If an icon is not provided, use "Page" as the default.   If a value is not provided for the columns View, Insert, Update, or Delete use True as a default value when generatng the Excel document.  If a value is not provided for the columns Hide from Navigation, Execute Search On Load, or Is Self Aware use False as a default value when generatng the Excel document.  For the Data Display Name column if data is not provided use the Name column and remove any spaces from it.

    Form Tab Columns:
    -   Name*
    -   Scope*
    -   Tags*
    -   Description*
    -   ImportData
    -   Icon*
    -   Header
    -   Footer
    -   Integration Code
    -   Sort Order*
    -   Data Display Name
    -   View
    -   Insert
    -   Update
    -   Delete
    -   Record Display Identifier
    -   Hide from Navigation
    -   Execute Search On Load
    -   Is Self Aware
    -   Email Controls


5.  Form filters are used throughout the application but not required.  On the Form filters tab the document must contain the following columns and make them bold if possible.  Anything with an asterisk is required from the user.  Also, tags are seperated by semicolons.

    Form Filters Tab Columns:
    -   Name*
    -   Form*
    -   Tags*
    -   Description*


6.  Form filter rows are children of form filters and they are the assingnmnets on the data to help filter.  They are not required however, if you have a form filter you should have form filter rows.  On the Form filter rows tab the document must contain the following columns and make them bold if possible.  Anything with an asterisk is required from the user.  Also, tags are seperated by semicolons.

    Form Filter Rows Tab Columns:
    -   Name*
    -   Form*
    -   Tags*
    -   Description*


7.  On the Controls tab we build out the controls/fields that will be on the form created before.  On the Controls tab the document must contain the following columns and make them bold if possible.  Anything with an asterisk is required from the user.  Also, tags are seperated by semicolons.

    Control Tab Columns:
    -   Form*
    -   Name*
    -   Scope*
    -   Tags*
    -   Description*
    -   Control Type
    -   Field Type
    -   Data Source
    -   Text Title
    -   Text Block
    -   Required
    -   Unique
    -   Prefix
    -   Suffix
    -   Tooltip
    -   Tab Name*
    -   Row*
    -   Column*
    -   Default Value
    -   Search Row
    -   Search Column
    -   Search Result Order
    -   Default Search Value
    -   Default Search Supporting Value
    -   Print Bookmark
    -   Integration Code
    -   Business Rule Name
    -   Data Display Name
    -   View
    -   Update
    -   Cascading Dropdown
    -   Cascading Child
    -   Parent Dropdown Field
    -   Cascade Grid Field
    -   View of Grid Data
    -   Grid Row Unique
    -   Hide Grid Add New
    -   Hide Grid Add Existing
    -   Grid Parent Form
    -   Grid Parent Field


8.  The next tab is actually called Tabs.  Tabs are required because they are used on Forms/Pages.  The Tabs tab must contain the following columns and make them bold if possible.  Anything with an asterisk is required from the user.  Also, tags are seperated by semicolons.

    Tab Tab Columns:
    -   Form*
    -   Name*
    -   SortOrder*


9.  The Dropdowns tab is used to configure static or form dropdowns.  They are only required if there are dropdown controls.  The Dropdowns tab must contain the following columns and make them bold if possible.  Anything with an asterisk is required from the user.  Also, tags are seperated by semicolons.

    Dropdown Tab Columns:
    -   Form*
    -   Name*
    -   Type*
    -   Data
    -   Filter


10. The Webhooks tab is used to build out any API calls you would like made after a specific event occurs.  The Webhooks tab must contain the following columns and make them bold if possible.  Anything with an asterisk is required from the user.  Also, tags are seperated by semicolons.

    Webhooks Tab Columns:
    -   Name*
    -   Tags*
    -   Description*
    -   URL*
    -   Await Return
    -   Form-Event


11. The Rules tab is used for any custom rules or error messages you would like to provide.  The tab is not required.  The Rules tab must contain the following columns and make them bold if possible.  Anything with an asterisk is required from the user.  Also, tags are seperated by semicolons.

    Rules Tab Columns:
    -   Name*
    -   Tags*
    -   Description*
    -   Expression*
    -   Rule Type*
    -   Error Message*


12. The Grids tab is used for create grids out of a specific forms data and then be used on a Control/Field.  The tab is not required.  The Grids tab must contain the following columns and make them bold if possible.  Anything with an asterisk is required from the user.  Also, tags are seperated by semicolons.

    Grids Tab Columns:
    -   Name*
    -   Description*
    -   Tags*
    -   Form*
    -   Compact
    -   Header Visible
    -   Items Per Page
    -   Display Format {{Field Name}}*


13. The Grid Columns tab is used on by a Grid to determine what data elements from the supplied form you want shown in the grid.  The tab is not required unless you have a Grid.  The Grid Columns tab must contain the following columns and make them bold if possible.  Anything with an asterisk is required from the user.  Also, tags are seperated by semicolons.

    Grid Columns Tab Columns:
    -   Grid*
    -   Field Name*
    -   Collapsible*
    -   Resizable*
    -   Padded*
    -   Min Width*
    -   Max Width*


14. The API Keys tab is used when you want to call our API to update data from a different application.  The tab is not required.  The API Keys tab must contain the following columns and make them bold if possible.  Anything with an asterisk is required from the user.  Also, tags are seperated by semicolons.

    API Keys Tab Columns:
    -   Name*
    -   Key*
    -   Expiration Date*
    -   Read Only*
    -   Forms*