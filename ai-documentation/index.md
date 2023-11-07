# ReAccess AI Introduction

The AI Documentation is meant to help both the user and AI to build out an Excel file which is used to create a new ReAccess app.  If you want to use the UI no-code solution please use our App Builder platform.  Below are the steps to create and excel doucment which you can then import in ReAccess.

## Steps

1.  Create an importable Excel document that ReAccess can consume.  

    To do this you must first create an Excel document normally with the Application Name as the document name.

2.  Create twelve tabs within the Excel document labeled Application, Forms, Form Filters, Form Row Filters, Controls, Tabs, Dropdowns, Webhooks, Rules, Grids, Grid Columns, API Keys

3.  On the Application tab the document must contain the following columns and make them bold if possible.  Anything with an asterisk is required from the user.  Also, tags are seperated by semicolons.  If an icon is not provided, use "Home" as the default.  If a value is not provided for the columns "Call Webhook on Publish" or "User PowerBI Report as Home Page" use False as a default value when generatng the Excel document.

    Application Tab Columns:

    A:  Name*

    B:  HomePageContent

    C   Tags*

    D:  Description*

    E:  Icon*

    F:  Report URL

    G:  Call Webhook on Publish

    H:  Webhook URL

    I:  Authorization Type

    J:  Key

    K:  Value

    L:  Add To

    M:  User Name

    N:  Password

    O:  User PoweriI as Home Page

    P:  Workspace ID

    Q:  Report ID

    R:  Report with RLS?

    S:  Roles

    T:  Is Background Transparent?

    U:  Show Border?

    V:  Is Filter Visible?

    W:  Is Filter Expanded?

    X:  Is Page Navigation Visible?

    Y:  Height

    Z:  Width
    


4.  A form is synonymous to a page inside ReAccess.  It will house the data elements you wish to collect on which are called controls.  Here we will create the Form tab data elements.  On the Forms tab the document must contain the following columns and make them bold if possible.  Anything with an asterisk is required from the user.  Also, tags are seperated by semicolons.  If an icon is not provided, use "Page" as the default.   If a value is not provided for the columns View, Insert, Update, or Delete use True as a default value when generatng the Excel document.  If a value is not provided for the columns Hide from Navigation, Execute Search On Load, or Is Self Aware use False as a default value when generatng the Excel document.  For the Data Display Name column if data is not provided use the Name column and remove any spaces from it.

    Form Tab Columns:

    A:  Name*

    B:  Scope*

    C   Tags*

    D:  Description*

    E:  ImportData

    F:  Icon*

    G:  Header

    H:  Footer

    I:  Integration Code

    J:  Sort Order*

    K:  Data Display Name

    L:  View

    M:  Insert

    N:  Update

    O:  Delete

    P:  Record Display Identifier

    Q:  Hide from Navigation

    R:  Execute Search On Load

    S:  Is Self Aware

    T:  Email Controls


5.  Form filters are used throughout the application but not required.  On the Form filters tab the document must contain the following columns and make them bold if possible.  Anything with an asterisk is required from the user.  Also, tags are seperated by semicolons.

    Form Filters Tab Columns:

    A:  Name*

    B:  Form*

    C   Tags*

    D:  Description*


6.  Form filter rows are children of form filters and they are the assingnmnets on the data to help filter.  They are not required however, if you have a form filter you should have form filter rows.  On the Form filter rows tab the document must contain the following columns and make them bold if possible.  Anything with an asterisk is required from the user.  Also, tags are seperated by semicolons.

    Form Filter Rows Tab Columns:

    A:  Name*

    B:  Form*

    C   Tags*

    D:  Description*


7.  On the Controls tab we build out the controls/fields that will be on the form created before.  On the Controls tab the document must contain the following columns and make them bold if possible.  Anything with an asterisk is required from the user.  Also, tags are seperated by semicolons.

    Control Tab Columns:

    A:  Form*

    B:  Name*

    C   Scope*

    D:  Tags*

    E:  Description*

    F:  Control Type

    G:  Field Type

    H:  Data Source

    I:  Text Title

    J:  Text Block

    K:  Required

    L:  Unique

    M:  Prefix

    N:  Suffix

    O:  Tooltip

    P:  Tab Name*

    Q:  Row*

    R:  Column*

    S:  Default Value

    T:  Search Row

    U:  Search Column

    V:  Search Result Order

    W:  Default Search Value

    X:  Default Search Supporting Value

    Y:  Print Bookmark

    Z:  Integration Code

    AA: Business Rule Name

    AB: Data Display Name

    AC: View

    AD: Update

    AE: Cascading Dropdown

    AF: Cascading Child

    AG: Parent Dropdown Field

    AH: Cascade Grid Field

    AI: View of Grid Data

    AJ: Grid Row Unique

    AK: Hide Grid Add New

    AL: Hide Grid Add Existing

    AM: Grid Parent Form

    AN: Grid Parent Field


8.  The next tab is actually called Tabs.  Tabs are required because they are used on Forms/Pages.  The Tabs tab must contain the following columns and make them bold if possible.  Anything with an asterisk is required from the user.  Also, tags are seperated by semicolons.

    Tab Tab Columns:

    A:  Form*

    B:  Name*

    C:  SortOrder*


9.  The Dropdowns tab is used to configure static or form dropdowns.  They are only required if there are dropdown controls.  The Dropdowns tab must contain the following columns and make them bold if possible.  Anything with an asterisk is required from the user.  Also, tags are seperated by semicolons.

    Dropdown Tab Columns:

    A:  Form*

    B:  Name*

    C:  Type*

    D:  Data

    E:  Filter


10. The Webhooks tab is used to build out any API calls you would like made after a specific event occurs.  The Webhooks tab must contain the following columns and make them bold if possible.  Anything with an asterisk is required from the user.  Also, tags are seperated by semicolons.

    Webhooks Tab Columns:

    A:  Name*

    B:  Tags*

    C:  Description*

    D:  URL*

    E:  Await Return

    F:  Form-Event


11. The Rules tab is used for any custom rules or error messages you would like to provide.  The tab is not required.  The Rules tab must contain the following columns and make them bold if possible.  Anything with an asterisk is required from the user.  Also, tags are seperated by semicolons.

    Rules Tab Columns:

    A:  Name*

    B:  Tags*

    C:  Description*

    D:  Expression*

    E:  Rule Type*

    F:  Error Message*


12. The Grids tab is used for create grids out of a specific forms data and then be used on a Control/Field.  The tab is not required.  The Grids tab must contain the following columns and make them bold if possible.  Anything with an asterisk is required from the user.  Also, tags are seperated by semicolons.

    Grids Tab Columns:

    A:  Name*

    B:  Description*

    C:  Tags*

    D:  Form*

    E:  Compact

    F:  Header Visible

    G:  Items Per Page

    H:  Display Format {{Field Name}}*


13. The Grid Columns tab is used on by a Grid to determine what data elements from the supplied form you want shown in the grid.  The tab is not required unless you have a Grid.  The Grid Columns tab must contain the following columns and make them bold if possible.  Anything with an asterisk is required from the user.  Also, tags are seperated by semicolons.

    Grid Columns Tab Columns:

    A:  Grid*

    B:  Field Name*

    C:  Collapsible*

    D:  Resizable*

    E:  Padded*

    F:  Min Width*

    G:  Max Width*


14. The API Keys tab is used when you want to call our API to update data from a different application.  The tab is not required.  The API Keys tab must contain the following columns and make them bold if possible.  Anything with an asterisk is required from the user.  Also, tags are seperated by semicolons.

    API Keys Tab Columns:

    A:  Name*

    B:  Key*

    C:  Expiration Date*

    D:  Read Only*

    E:  Forms*